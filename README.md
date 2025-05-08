# HTML, CSS


## 1. HTML 기본구조

```HTML
<!DOCTYPE html>

<html lang="en">

  <head>
    <meta charset="UTF-8" />
    <title>Title</title>
  </head>

  <body>
  contents
  </body>

</html>
```


### 1.1. <>와 </>
- 어떤 요소의 시작은 <>로 시작하고 끝은 </>의 형식

### 1.2. 문서 타입 선언
```HTML
<!DOCTYPE html> 
```
- 해당 문서가 HTML5로 작성 되었다는 것을 나타냄

### 1.3. 문서의 시작과 끝
```HTML
<html lang="en">
</html>
```
- html 문서의 시작이며, </html> 태그가 있는 곳이 문서의 끝 
- lang 속성으로 문서가 어떤 언어로 구성되어 있는지 표기

### 1.4. head요소, title요소
```HTML
<head>
    <meta charset="UTF-8"/>
    <title>Title</title>
</head>
```
- head요소는 문서 내용에는 반영되지 않음
- 브라우저에 문서의 정보를 전달하는 역할
- head요소 내부에 Title요소를 사용해 내용을 감싸면 브라우저의 탭에 해당 내용이 표시됨

### 1.5. body요소
```HTML
<body>
contents
</body>
```
- body요소 안의 내용은 브라우저 윈도우에 표시되는 내용
- 실제로 눈에 보이는 내용은 body요소 내부에 있어야 함

## 1.1 HTML의 다양한 요소

### 1.1.1 Paragraphs요소
```HTML
<p>안녕하십니까 저는 대학생 이승민입니다</p>
<p>현재 대학교에 재학중이며, 컴퓨터와 관련된 여러가지를 배우고 있습니다</p>
```
- 본문 내용을 작성할때 사용하는 요소

### 1.1.2 Headings요소
```HTML
<h1>계명대학교</h1>
<h2>컴퓨터공학과</h2>
<h3>web construction</h3>
```
- h1부터 h6까지 사용가능하며 문서의 머리 부분이다
- 주로 제목, 주제, 서두에 사용함

### 1.1.3 리스트 요소
#### 1. Unordered lists
```HTML
<ul>
  <li>계명대학교</li>
  <li>컴퓨터공학과</li>
  <li>web construction</li>
</ul>
```
- 계명대학교
- 컴퓨터공학과
- web construction

- 이런식으로 결과는 점만 찍히는 리스트이다

#### 2. ordered lists
```HTML
<ol>
  <li>계명대학교</li>
  <li>컴퓨터공학과</li>
  <li>web construction</li>
</ol>
```
1. 계명대학교
2. 컴퓨터공학과
3. web construction

- 이런식으로 순차적 숫자가 반영되는 리스트이다

#### 3. Discription lists
```HTML
<dl>
  <dt>계명대학교</dt>
  <dd>아름다운 학교</dd>
</dl>
```

<dl>
  <dt>계명대학교</dt>
  <dd>아름다운 학교</dd>
</dl>

- 어떤 것을 설명하기 위한 리스트

### 1.1.4 img요소
```HTML
<img src="images/photo.jpg" alt="Seungminnni" title="seungminLee profile Photo" 
width="600" height="450" />
```
- 이미지 첨부할때는 ```<img src/>```를 사용한다
- src는 이미지 소스의 주소넣는다
- alt는 이미지의 설명을 제공한다
- title은 추가적인 이미지의 정보를 제공하며 마우스를 이미지에 호버했을때 설명이 띄워진다
- width와 height는 이미지의 너비와 높이를 지정한다

### 1.1.5 글씨에 하이퍼링크 삽입하기
```HTML
<a href="https://www.kmu.ac.kr/">KMU</a>
```
- ```<a href="사이트 링크">내용</a>``` 형식으로 작성
- 내용이라는 글씨를 클릭하면 사이트 링트로 이동 됨
- 실제로 적용된 예시
<a href="https://www.kmu.ac.kr/">KMU</a>

## 1.2 사용예시
### 1.2.1 리스트요소와 하이퍼링크기능 같이 사용해보기
```HTML
<ul>
  <li><a href="https://www.kmu.ac.kr/">KMU</a></li>
  <li><a href="https://www.kmu.ac.kr/">YU</a></li>
<ul>
```
- 큰 요소 내에 작은 세부요소 사용가능

## 2. CSS
- 작성한 HTML의 내용을 CSS를 이용해 꾸미거나 스타일을 변경
- 주로 외부스타일 시트를 이용한 방법을 사용함
- CSS파일 별도 관리, 여러 요소에 동일한 스타일 적용 가능, HTML과 CSS의 역할 분리로 가독성 향상
```css
body {
    font-family: Arial, sans-serif;
}
h1 {
    color: blue;
}
```
- 해석하면, body요소는 폰트를 Arial, sans-serif로 적용한다는 의미 h1요소는 색깔을 파란색으로 적용
- 각 요소들에 대한 속성만 잘 안다면, 어렵지 않게 사용가능

## 2.1 CSS 적용 방법

### 2.1.1 외부 스타일시트 불러오기
```HTML
<head>
    <link rel="stylesheet" href="style.css">
</head>
```
- head요소 안에 작성하여 .css파일을 링크로 불러오기를 통해 선언한 스타일을 HTML내용에 적용시킬 수 있음


### 2.1.2. 내부 스타일시트 불러오기
```HTML
<head>
    <style>
        body { background-color: white; }
        p { color: black; }
    </style>
</head>
```
- style요소를 이용해 내부에서 바로 스타일 적용

### 2.1.3. 인라인 스타일 적용
```HTML
<p style="color: blue; margin-left: 20px;">This is a paragraph.</p>
```
- 각 요소에 바로 스타일 적용

