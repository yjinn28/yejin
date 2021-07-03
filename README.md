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
> 
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

> 포함관계(nested)로 구성된 목록 - 코딩할 때 밖에서 안쪽 방향 순서로 코딩
- HTML
  - HTML4
  - HTML5
 - CSS
   - CSS2
   - CSS3
```
<ul>
  <li>
    HTML
    <ul>
      <li>HTML4</li>
      <li>HTML5</li>
    </ul>
  </li>
  <li>
    CSS
    <ul>
      <li>CSS2</li>
      <li>CSS3</li>
    </ul>
  </li>
```

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

> 북마크 기능
> 
> 외부 페이지 연결이 아닌 같은 페이지에서 특정 위치로 이동할 수 있게 해주는 기능
> 
> 도착지점에 id attribute를 사용하여 이름을 지정
```
<a href="#t1"></a>
...
<h2 id="t1">제목</a>
```

### Table Element

> 기본 사용 태그 : table, thead, tbody, tr, th, td 
> 
> 열 제목 (표 제일 위에 있는 카테고리 이름) : thead(table head), th(table heading)
> 
> 표 내용 : tbody(table body), td(table data)
> 
> 행 : tr(table row) -> 물리적인 한 줄
> 
https://www.tablesgenerator.com/html_tables#

### Image Element

> Tag : img (종료 태그 없음)
> 
> Attribute : src(image 위치, 파일명), alt(대체 텍스트)
> 
` : backtick이라고 부름
```
<img src="image.jpg" alt="대체텍스트">
```

### Video Element

> 비디오 및 오디오 콘텐츠는 용량이 크기 때문에 서버에 저장해서 콘텐츠를 제공하면 많은 트래픽이 발생할 수 있음.

> 트래픽 과부하를 해결하기 위해서 유튜브 서비스를 사용하기도 함.
> 
> attribute
> 
> controls : 컨트롤 버튼 표시

> autoplay : 자동 재생(* muted와 같이 사용해야 함)

> muted : 음소거

> loop : 반복 재생

### Youtube

> 비디오 콘텐츠 제공시 서버의 트래픽 과부하를 해결할 수 있는 방법 중의 하나

> 매개변수

> controls=1, 0

> autoplay=1, 0

> mute=1. 0

> loop = 1, 0(playlist와 함께 사용)

> 이미지와 동영상, 오디오 콘텐츠는 외부에서 만들어지는 콘텐츠 -> 이미지, 동영상, 오디오는 직접 입력하는 것이 아니고 외부 파일을 삽입 => 임베드(embed) 콘텐츠

> 텍스트는 HTML 문서에 직접 입력되는 콘텐츠

### 웹사이트 디자인 사이트

> https://freebiesbug.com/psd-freebies/minimo-minimal-blog-template/

### Container Elemet (단순 영역 구분 요소)

> div(division)

> span

### Block, Inline

> block Element, Inline Element 구분은 영역 화면 표시 방식에 따른 구분 
> 
> 모든 Element는 각각의 고유 영역을 가지고 있음

> 시각적인 기준에 따라 Block, Inline으로 구분됨
> 
> block Element는 줄바꿈 되어 표시 - block Element 영역의 가로 너비가 부모요소에 100% 채워짐
> 
> block Element에는 위, 아래 여백을 적용할 수 있음

> inline Element는 같은 줄에 나란히 표시 - inline Element 영역의 가로 너비가 콘텐츠 크기만큼만 채워짐

> inline Element는 위, 아래 여백을 적용할 수 없음

### Parent Element(부모요소), Child Element(자식요소)

> 포함관계에서 포함하는 요소가 부모요소, 포함되는 요소가 자식요소
> 직계 포함관계에서만 부모요소, 자식요소
> 직계가 아닌 포함관계에서는 조상요소, 자손요소


### CSS 기본 개념

> 선택자는 스타일을 지정할 HTML 요소를 가리킨다.

> 선언 블록에는 세미콜론으로 구분된 하나 이상의 선인이 포함된다.

> 각 선언에는 콜론으로 구분된 CSS 속성(property) 이름과 값(value)이 포함된다.

> 여러 CSS 선언은 세미콜론으로 구분하고 선언 블록은 중괄호로 묶는다.

> html 속성 : attribute
> css 속성: property

### id, class

> HTML element에 특정 이름을 사용할 때 id, class attribute를 사용해서 이름을 붙여줄 수 있음.
> 
> id는 동일한 이름이 사용된 HTML element가 여러 개이면 논리적 오류가 발생
> 
> id는 HTML 문서 내에서 고유해야 함.

> class는 동일한 이름이 여러 개의 element에 사용되어서 공통 디자인 요소나 공통 기능을 적용할 수 있음.
> 
> id는 주로 서버에서 불러오는 데이터를 표시하는 위치에 고유하게 사용 ==> 백엔드 개발에서 주로 사용
> 
> class는 주로 css 스타일 적용, javascript 인터랙션 적용하 때 사용 ==> 프론트엔드 개발에서 주로 사용

### CSS 작성 방법

> External class : 파일 분리

> Internal class : 같은 HTML 문서 내에 head 태그 영역에 <sytle> 태그를 사용하여 입력
  
> Inline CSS : 시작 태그에 sytle attribute를 사용해서 입려 => javascript에서 CSS를 제어할 때 사용
  
  
### naming할 때 표기 방식
  
> id/class naming, 변수/함수 naming, 파일/폴더 naming의 경우 가독성을 높이기 위해 사용
  
> 표기방식을 사용하는 이유
> - naming 할 때 두단어 이상으로 경우 단어와 단어 사이를 구분하기 위해 사용
> - 단어의 시작 부분에 첫글자를 대문자로 변경, 특수 기호를 사용 
> 
> 표기방식 종류
> 
> snake case : gnb_depth1 => 파일/폴더
> 
> kebab case : gnb_depth1 => id/class
> 
> camel case : gnbDepth1 => javascript의 변수/함수
> 
> Pascal case : GnbDepth1 => javascript의 클래스

  
  
  
  
