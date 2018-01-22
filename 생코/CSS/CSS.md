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
