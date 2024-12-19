### 01. img 태그에 대하여 알아보기

1) img 태그는 이미지를 호출할때 사용되는 태그이다.

2) 인라인 요소에 해당하는 태그그

3) 호출시 src 속성을 통해 주소를 연결하고,
    alt를 이용하여 글을 작성한다.

---

### 02. alt 를 작성하는 이유는?

	예를 들어 src에 연결된 이미지 파일이
    01.jpg 파일 이라면... 
    어떤 이미지 파일인지 알수가 없다..

    이럴 경우를 대비하여 alt를 통해 어떤 이미지인지 대체할 텍스트를 작성한다.
    (웹표준에도 속하기 때문에 매우 중요하다.)

---

### 03. img 태그로 호출한 이미지

![headline.html](img/background0.jpg)

---


### 04. 코드확인

> img-tag.html

```html


<!DOCTYPE html>
<html lang="ko">
 <head>
  <title>img-tag</title>
  <meta charset="utf-8"/>

 <body>
	<h2>이미지 설정하기</h2>
	<hr/>
	<p>
		<img src="img/background0.jpg" alt="일러스트 꽃 이미지"/>
	</p>
 </body>
</html>

```