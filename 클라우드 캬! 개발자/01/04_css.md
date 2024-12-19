### 01. css의 종류

1) 인라인 스타일 적용방식 (inline-style)
2) 내부 적용방식 (internal-style)
3) 외부 적용방식 (external-style)
---

### 02. 각각의 적용방식의 사용법
1) 인라인 스타일 적용방식은 태그에 직접적용
2) 내부 적용방식은 style 영역을 만들어서 적용
3) 외부 적용방식은 외부 파일로 스타일 영역을 분리 하여 적용

---

### 03. 인라인 요소와 블록요소에 css 적용후 확인

인라인 요소은 타이트하게 자신의 범위까지만
표현되지만, 블록요소는 끝에서 끝까지 영역을
차지하는 것을 알 수 있음

> 참고이미지

![headline.html](img/inline-block-area.jpg)

---

### 04. 각각의 css 적용방법의 장,단점 



---

### 05. 아래 코드를 보고 문제풀면서 시각적으로 확인하기


**1) 내부 적용방식 (internal 방식)**

>장점

현재 페이지에서 stylesheet 영역을 만들어 표현하는 방식으로 사용자가 빨리 확인할 수 있고, 자주 수정이
가능하다.

> 단점

1. 기능이 복잡해지거나 꾸며줄 요소가 많아지면 코드를 한번에 보기가 어려워진다.

2. 한 페이지 내에 읽어야 하는 값들이 너무 많아져 느려
질수 있다.



**2) 외부 적용방식 (external 방식)**

>장점

1) stylesheet를 따로 분해하여 작업하는 방식으로 팀 작업시 원하는 파일만 보낼 수 있다.

2) 각각의 영역마다 따로 분해하여 작업이 가능하다.
3) 태그와 style을 분해하여 정리할때 매우 편리하다.

>단점

1) 분실의 우려가 있다.
2) 다른 팀원에 의해 변질될 수 있다.


**3) 인라인 적용방식 (inline 방식)**

>장점

1) 태그에 적집 적용하는 방식으로, 내부적용 방식, 외부적용 방식 어떤 것에도 영향을 받지 않는다.

2) 주로 "하나의 객체에 유일" 하게 효과를 적용하거나 기능을 부여할 때 주로 사용하면 좋다.

> 단점

10개, 100개, 1000개 이상의 객체 동일하게 대량작업이 어려움!

---

> 04_css.html

```html



<!DOCTYPE html>
<html lang="ko">
 <head>
  <title>css</title>
  <meta charset="utf-8"/>
  <style>

		p{background-color:pink;}
		#orange{background-color:orange;}

		/*
			[응용문제]

			1) h3태그 호출하여 배경색상 gold로 변경하기, 글자 색상은 파란색 적용하기

			2) h2 태그들 중에서 " 블록요소, 인라인요소 " 라고 제목 작성되어 있는 
			태그만 호출하여 배경색상 빨간색, 글자색상 하얀색 적용하기!
		*/

		h3{background-color:gold; color:blue;}
		#hh2{background-color:red; color:white;}

  </style>
 </head>

 <body>
	<h2>태그에 직접 적용하는 방식 : inline-style 적용방식</h2>

	<h3>응용문제1</h3>
	<p style="background-color:blue;">현재 p태그에 배경색상 파란색 적용하기</p>
	<p style="color:green;">현재 p태그에 글자색상 초록색 적용하기</p>
	<p style="background-color:pink; color:green;">현재 p태그에 배경색상 pink, 글자 색상 초록색 적용하기</p>

	<h3>응용문제2</h3>
	<p style="background-color:gray;">
		현재 p태그의 배경색상 gray 적용하기<br/>
		<span style="color:blue;">현재 span태그에 글자색상 파란색 적용하기</span><br/>
		<span style="background-color:yellow;">현재 span태그에 배경색상 노란색 적용하기</span>
	</p>

	<h2 id="hh2">블록요소, 인라인요소</h2>
	<p>
		인라인 속성은 위의 span 태그처럼 글자가 가진 크기 만큼만 영역을 차지하는 것을 알 수 있음<br/>
		블록속성은 위의 p태그를 확인해보면 gray 색상이 끝에서 끝까지 차지하는 것을 알 수 있음<br/>
		<strong style="background-color:aqua;">인라인은 담고 있는 객체 만큼만 타이트하게 , 블록은 처음부터 끝까지 영역을 차지함</strong>
	</p>
 </body>
</html>

```