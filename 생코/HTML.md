# HTML
Hyper Text Markup Language의 약자
하이퍼텍스트를 가장 중요한 특징으로 하는 마크업 형식의 프로그래밍 언어


```html
<strong> 시작태그
</strong> 닫히는 태그

<h1> 헤드1. 줄 바꿈은 자동
<h1>~<h6>까지 있음

<a>태그만 달면 아무런 변화가 없다. 정보가 불충분해서 URL을 달아줘야함
<a href="블라블라"> 링크를 거는 태그
<target="_blank"> 새창으로 여는 태그
    <a target="_blank" href="블라블라"> 이렇게 달아도 됨
    <title> 툴팁
        
        
        
***태그를 중첩해서 사용하기
목록을 구성할 때는 리스트 태그를 사용한다
<li>태그는 보통 단독으로 쓰지않는다. list
<ul>로 묶어주어 그룹핑한 효과를 낸다. unordered list
<li>단독으로는 성격을 다르게 구분하는 효과를 낼 수 없다.
<ol>은 숫자 리스트가 됨. ordered list

<tilte>과 <meta charset>은 본문이 아닌 부가적인 정보를 넣는다
보통 <head>에 들어가도록 약속되어있고 본문은 <body>에 들어간다

html의 문서는 이런 구조를 가지고 있다
<html>
    <head>
    </head>
    <body>
    </body>
</html>



<!DOCTYPE html>
도큐먼트 타입
어떤 방식의 html코드로 작성되었는지 브라우저에게 알려주는 것(선언하는 것)
브라우저는 태그같은 게 어떤 표준에 따라 제정된 것인지 알 필요가 있기 때문이다



***html 변천사
웹이 발전하면서 태그가 늘어남
http://www.martinrinehart.com/frontend-engineering/engineers/html/html-tag-history.html

***구글의 HTML 통계
https://www.advancedwebranking.com/html/
많이 쓰는 태그나 속성을 볼 수 있음



***태그 공부
<p>
paragraph의 줄임말로 단락을 표현할 때 사용한다
html은 줄바꿈을 무시하기 때문에 브라우저에게 단락을 구분시켜야한다
단락의 시작과 끝에 <p>태그를 감싸준다
<p>태그는 높이 간격을 css로 수정할 수 있음



<br>
<p>태그를 써도 되지만, 줄바꿈의 간격이 고정되어있기 때문에.
<br>태그는 열리는 태그 하나만 마지막 단락에 써주면 됨
<p>태그는 2줄의 줄바꿈이 되는데 <br>은 2번 입력하면 같은 모습이 됨
그러나 <br>태그는 시각적인 걸 표현하는 거고, <p>는 하나읟 단락이라는 '정보'를 표현할 수 있다. css로 간격을 조정하는 게 나중에 더 좋을거다~



<img>
width="200" 
height="200"
이런 식으로 사이즈 변경도 가능
alt : 이미지가 깨졌을 때 뜨는 대안문구
title 태그를 이용해서 툴팁을 만들 수 있음


 




-HTML의 변천사와 통계까지 봄