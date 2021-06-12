# HTML, CSS, JS 기초

## HTML

> HTML : Hyper Text Markup Language - 마크업(표시) 언어

> 웹페이지의 구조를 표시

> 웹페이지의 콘텐츠를 표시

## HTML Elements

> Element : 요소 - 의미적

> Tag : 태그 - 기술적

> 문법(Syntax)
> 
> <>로 감싸줌
> 
> 소문자로 사용
> 
> 시작태그와 종료태그 세트로 구성됨
```
<tagname>contents</tagname>
```
> 
> 예외) 시작태그만 존재하는 경우 : 빈 요소(Empty Element)
> 
> 포함관계(Nested)
```
<body>
  <div>
    text
  </div>
</body>
```

### HTML Attribute

> HTML 속성
> HTML 요소의 부가 정보
> 속성이름= "속성값"

```
<a href="http://www.naver.com">naver</a>
```

### 제목 태그

> heading -> h
> h1 ~ h6
> h1이 가장 큰 제목

### HTML 기본 구조

```
<!DOCTYPE html> - 1
<html> - 2
  <head> - 3
    <meta charset="utf-8"> - 4
    <title>My test page</title> - 5
  </head>
  <body> - 6
    <p>This is my page</p>
  </body>
</html>
```

1. 웹 문서의 버전 : HTML5
2. HTML 문서의 가장 바깥쪽 요소(가장 밖에서 포함하고 있는 것이므로 바깥쪽 요소라고 말함)
3. 웹 문서를 설명하는 정보가 담기는 영역 요소
4. 웹 문서의 정보를 표시하는 요소
5. 웹 문서의 제목을 표시하는 요소(상단 탭에 보이는 제목)
6. 웹 문서의 콘텐츠 요소들이 담기는 영역 요소

### 단락 태그

> p(Paragraph) : 단락을 표시
> 단락과 단락 사이를 구분하는 수평선
```
<hr> - horizontal rule
```
> 단락을 구분하지 않고 줄 바꿈
```
<br> - break
```
### 목록 태그

> 순서 없는 목록 ul(Unordered List)
> 순서 있는 목록 ol(Ordered List)
> 목록 항목 li(List Item)

```
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>HTML</li>
  <li>CSS</li>
</ol>
```

> 포함관계로 구성된 목록
- HTML
  - HTML4
  - HTML5
 - CSS
   - CSS2
   - CSS3

> 설명목록(Description List) - dl

```
<dl>
  <dt>HTML</dt> (dt : Description Title)
  <dd>표준 마크업 언어</dd> (dd: Description Data/dt를 설명하는 역할)
</dl>
```

### HTML Hyper link

> 하이퍼링크 a(anchor)

> attribute(속성) : href(Hypertext Reference) : 연결되는 웹 문서의 URL
```
<a href="http://www.naver.com">네이버로 이동</a>
```






