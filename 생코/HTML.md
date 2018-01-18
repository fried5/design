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


 
 
<table>
태그 중에 어려운 측에 속함
       <table border="1">
       <tr>
           <td>이름</td> 
        </tr>
        </table>
테이블 자체는 cSS로 꾸며줌
td = table data
tr = table row

예전에는 웹페이지 전체를 표로 잡고, 안에 박스단위로 다 표로 잡았음
하지만 table은 레이아웃을 잡으라고 만든 태그가 아님.
엑셀같은 정보구조를 만드는데 쓰는 태그임
table로 짜면 html이 너저분하게 됨


<thead></thead>
<tbody></tbody>
로 정보제목?과 내용을 구분해줌
사람이 안하면 브라우저가 자동으로 함
<td>태그는 <th>로 바꿔줄 수 있는데 이렇게하면 진하게 표시된다
tfoot은 무조건 아래로 내려감






<form>
서버로 보내기위한 정보들을 입력하는 폼
   아이디 : <input type="text" name=id">
   비밀번호 : <input type="password" name="pwd">
   제출버튼 <input type="submit">
   <form action="http://localhost.php">
form태그를 통해 로그인 정보를 어디로 보낼지 정할 수 있다.
서버에 대해 몰라도 주소를 알면 됨
name을 붙여서 보내면 서버에서 네임값이 붙어서 전송받게 됨

value=""
인풋폼에 뭔가 미리 적혀있도록 함
textarea cols="50" row="10"
여러 줄을 입력할 수 있는 폼인데 50글자의 폭과 10줄을 입력할 수 있는 크기로 지정






-HTML의 변천사와 통계까지 봄