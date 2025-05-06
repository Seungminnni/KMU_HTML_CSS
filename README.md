# HTML, CSS


## 1. HTML 기본구조

```html
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
```
<!DOCTYPE html> 
```
- 해당 문서가 HTML5로 작성 되었다는 것을 나타냄

### 1.3. 문서의 시작과 끝
```
<html lang="en">
</html>
```
- html 문서의 시작이며, </html> 태그가 있는 곳이 문서의 끝 
- lang 속성으로 문서가 어떤 언어로 구성되어 있는지 표기

### 1.4. head요소, title요소
```
<head>
    <meta charset="UTF-8"/>
    <title>Title</title>
</head>
```
- head요소는 문서 내용에는 반영되지 않음
- 브라우저에 문서의 정보를 전달하는 역할
- head요소 내부에 Title요소를 사용해 내용을 감싸면 브라우저의 탭에 해당 내용이 표시됨

### 1.5. body요소
```
<body>
contents
</body>
```
- body요소 안의 내용은 브라우저 윈도우에 표시되는 내용
- 실제로 눈에 보이는 내용은 body요소 내부에 있어야 함

## 2. CSS

