# CSS
HTML은 전자출판을 위해 만들어진 언어
곧 HTML의 본질은 '정보'
어떻게 잘 정보를 표현할 것인가가 제일 큰 목적
정보와 디자인이 완전히 분리되었고 디자인의 역할을 CSS가 하게 됨


## 선택자
```
태그 선택자 : li{}
클래스 선택자 : .active{}
아이디 선택자 : #select{}
id선택자는 딱 한번만 쓰는 식별자임. 
이걸 쓰고나면 다른데다가는 select를 쓰면 안되기로 약속함.
반면에 class는 여러개를 그룹핑하는 성격을 가짐

ul li{}
띄어쓰기를 하면 ul밑에 li가 있다는 뜻임

#lecture>li
id가 lecture인 녀석의 직계자손인 li에 CSS를 주겠다
but.color는 상속의 성격도 추가로 가짐

ul,ol{}
,는 동등한 관계
```

## 선택자 팁
http://flukeout.github.io/

## CheatSheet
힌트를 얻을 수 있는 커닝페이퍼를 검색할 수 있음



## 가상 클래스 선택자
클래스 선택자처럼 행동하지만 클래스 선택자는 아닌 선택자
(엘리먼트의 특성에 따라 클래스 선택자처럼 몇몇 태그를 그룹핑한다.)
- hover, active, link, visited등(visited는 보안상의 문제 때문에 일부 속성만 사용 가능)
태그에서 위에 있는 것이 우선순위가 높다.
active가 제일 밑으로

:link - 방문한 적이 없는 링크
:visited - 방문한 적이 있는 링크
:hover - 마우스를 롤오버 했을 때 
:active - 마우스를 클릭했을 때

## 다양한 선택자
A,B  둘다 선택하는 것
*  웹페이지에 있는 모든 태그
A *  A의 모든 태그
A+B는 A의 옆에 있는 B가 선택됨. 바로 옆에 있는 것만 선택됨
A~B A에 인접해있는 B의 모든 것
A>B 엘리먼트의 직계자손을 선택한다. B중에 A의 바로 직계인 것만 선택된다.
B A:first-child B밑에 있는 A중에 첫번째로 등장하는 것을 선택
A:only-child 형제자매가 있는 애들은 선택되지 않고, 온니 차일드들만 선택된다
A:last-child 제일 뒤에 있는 엘리먼트 (.table>*:last-child)
plate:nth-child(3)  plate의 3번째 차이들
:nth-last-child(A) 뒤에서부터 숫자를 셈
:nth-of-type(A) A번째 등장하는 타입, odd와 even로 짝수/홀수 적용할 수도 있음
:nth-of-type(An+B) n의 변수는 컴퓨터가 넣는다. 
:nth-of-type(2n) 을 넣으면 2,4,6,8 등으로 선택된다.

특수한 선택자들 중에 4번째 강의는 다음에 들어야겠음.



## 속성에 대한 통계
https://developer.microsoft.com/en-us/microsoft-edge/platform/usage/



## font-size
단위는 크게 3가지인데 px / em / rem.
rem은 최근 추가된 단위.
px은 절대적인 크기, em와 rem은 상대적인 가변적인 크기이다.
오늘날에는 다른 걸 써야하는 이유가 분명하지 않으면 rem을 쓰면 된다고 보면 된다. = 폰트크기를 조정할 수 있는 사용자의 권리
사용자가 브라우저의 폰트 크기를 키웠을 때 px은 바뀌지않고 em은 rem은 바뀐다.

## Color
color name, hex, rgb으로 구성됨
https://www.w3schools.com/css/css_colors.asp


## font-align
left
right
center
justify : 자간이 가변적으로 바뀌면서 양옆이 균등하게 분배된다



## font-family
``
font-family: arial, verdana, "Helvetica Neue" serif monospace;
font-weight: bold;
line-height: 2;
 
글자마다 가변폭이 있는데, 정보를 다루거나 할 때 고정폭이 필요할 때 monospace
font-weight의 기본값은 1.2
line-height는 줄과 줄 사이의 간격. px을 줄 수도 있다. 하지만 상대적인 수치를 사용하는 것을 권장한다.
폰트에 관한 프로퍼티는 순서를 지켜서 작성해야한다.
font-style 
font-variant 
font-weight 
font-size/line-height 
font-family|caption|icon|menu|message-box|small-caption|status-bar|initial|inherit; 


## 웹폰트
폰트를 서버에서 다운로드하는 방식. 
한글같은 경우는 용량이 상당히 크다
구글폰트에서 @import 부분은 html head부분에 넣는다
style쪽에 specify in CSS를 넣는다

font face genertator라는 것을 통해서 웹폰트로 변환한다
다양한 브라우저에 대응할 수 있는 폰트를 만들어준다
@font-face라는 것을 통해 폰트파일에 대한 설명을 나열하고 정의한다
font-family에 동일하게 적어줘야한다.
(아직 로컬 폰트를 정확하게 어떻게 쓴다는 건지 이해못하겠음)


## 상속
주석쓰는 법 /* */
부모가 하는 걸 자식이 물려받는 게 효율적일 수 있다.
많은 것들 중에 몇개만 다르다면, 몇개에 id를 줘서 변경하는 게 더 효율적.
검사에서 보면 inherited from html이라는 것을 보고 상속받았다는 걸 확인할 수 있다.
속성 모두가 상속되는 것은 아니다. 
예를 들어 font color는 상속되지만 border는 상속되지않는다.

https://www.w3.org/TR/CSS21/propidx.html
css2의 여러 속성을 볼 수 있다.

## Stylish
CSS를 수정하거나, 남이 수정한 디자인을 내 컴퓨터에 적용할 수 있는 플러그인
플러그인을 통해 사이트를 커스터마이징할 수 있다.
디스케이딩으로 다른 cSS때문에 적용이 안된다면, cSS 뒤에 !Important라고 붙인다.


## Cascading
Cascading Style Sheet
### 우선순위
웹브라우저 < 사용자 < 저자

### CSS우선순위
태그선택자 < class선택자 < id선택자 < style속성
가장 포괄적인 규칙, 일반적인 것 < 구체적이면서 명시적인 규칙

"!important"라는 키워드를 넣으면 모든 것을 무시하고 우선순위가 가장 높아진다.