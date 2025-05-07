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

