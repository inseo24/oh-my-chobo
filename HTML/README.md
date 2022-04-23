# HTML5

# 기본 용어 정리

## 태그(tag)와 요소(element)

태그는 시작 태그와 닫는 태그로 이뤄집니다. 태그 사이에 담으려는 컨텐트가 들어가고 태그와 컨텐트 모두를 합쳐 요소(element)라고 합니다.

- 태그 + 컨텐트 = 요소(element)

```html
<h1>Hello HTML5</h1>
<!-- <시작태그> 컨텐트(내용) </끝(닫는) 태그> -->
```

## 속성(attribute)

태그의 추가 정보를 속성이라 합니다.

- 속성 이름 = “속성 값”

```html
<h1 title=”header”>Hello HTML5</h1>
```

## 주석(comment)

코드에 대한 설명을 쓰거나 코드를 사용하지 않게 처리할 때 사용합니다.

```html
<!-- 주석입니다 -->
```

여기서 실습을 한 번 해볼까요!

**HTML/1-1.html 코드를 참고해봅시다!**

**코드를 Live Server로 확인해보세요!**

**(코드 입력 창에서 마우스 오른쪽 버튼 누르면 Open with Live Server 버튼 클릭!)**



# HTML5 페이지 구조

HTML 요소들은 계층구조를 갖습니다.


- <html lang=”ko”>
    - 한국 : ko, 미국 : en, 일본 : ja, 중국 : zh ...
    - head 태그 내부에 넣을 수 있는 태그
    
    | 태그 이름 | 설명 |
    | --- | --- |
    | meta | 웹 페이지의 추가 정보로 전달 |
    | title | 웹 페이지의 제목 |
    

# 글자 태그

## 제목(header)

- h1 ~ h6
- 각각의 숫자는 크기를 나타낸다. 크기가 작을수록 글자가 커진다.
- 일반적인 웹페이지에서는 h1 ~ h3을 사용한다.

**여기서 HTML/1-2.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

## 본문(paragraph)

- p 태그
- 한 단락을 만듭니다.

- br : 줄바꿈 태그
- hr : 수평 줄을 만드는 태그

**여기서 HTML/1-3.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**
    
## 기본 목록

- ul : 순서가 없는 목록 태그입니다. unordered list의 줄임말입니다. 글머리 기호 생각하면 됩니다.
- ol : 순서가 있는 목록 태그입니다. ordered list의 줄임말입니다.
- li : 목록 요소입니다. list item입니다.

**여기서 HTML/1-4.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**
    
## 시맨틱 태그(semantic)

- semantic: 검색 엔진에서 태그를 분석해서 컨텐츠를 뽑을 수 있게 합니다. 일반 태그보다는 아래 태그를 쓰는게 검색 했을 때 더 검색에 잘 노출된다고 생각하면 됩니다!
    - header: 헤더를 의미
    - nav: 내비게이션을 의미
    - aside: 사이드에 위치하는 공간을 의미
    - section: 여러 중심 내용을 감싸는 공간을 의미
    - article: 글자가 많이 들어가는 부분을 의미
    - footer: 푸터를 의미
    - 등등
    
**여기서 HTML/1-5.html 코드를 참고해보세요!**
**코드를 Live Server로 확인해보세요!**
    

이제 기본적인 HTML 태그를 이용해 간단히 웹사이트를 만들어볼까요!
homework.md 파일을 참고해주세요! (나무위키.html 도 같이 확인^ㅁ^)



# Anchor/Image 태그

## Anchor Tag

1. 앵커 태그
    - a : 앵커 태그(링크)
    - 새로운 웹페이지로 이동하거나 사이트 내부에서 특정한 위치로 이동할 때 사용하는 태그
    - href 속성 값에 “#요소의ID”를 넣어 설정

**여기서 HTML/1-6.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

## Image Tag

1. 이미지 태그
    - img 태그의 속성
        - src: 경로 지정
        - alt : 이미지가 없을 때 나오는 글자 지정
        - width: 이미지의 너비
        - height: 이미지의 높이 지정

이미지를 지정하는 방법에는 3가지가 있습니다.

1. 내부 파일을 지정하는 방법
2. 외부 파일 링크를 이용하는 방법
3. 데이터 URL 방식이 있습니다.
    1. HTTP 요청을 절약할 수 있고 HTML 파일로 관리할 수가 있다는 장점이 있습니다.
    2. 기존 파일보다 용량이 커진다는 단점이 있습니다. 또한 base64 인코딩 같이 추가 작업으로 인해 메모리, 처리 시간으로 성능 저하가 발생할 수 있습니다.
    3. “data:image/jpeg;base64” 로 시작합니다.
    4. data 형식의 jpeg인 image며 base64로 인코딩되어 있다는 뜻입니다.

**여기서 HTML/1-7.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

[이미지 파일 Data URL 변환기](https://wepplication.github.io/tools/img2Url/)를 이용해보세요!

# 테이블, 공간 분할 태그

## 글자 태그 - 글자 형태

- b, strong: 굵은 글자 태그
- i, em: 기울어진 글자 태그
- small: 작은 글자 태그
- sub: 아래에 달라 붙는 글자 태그
- sup: 위에 달라 붙는 글자 태그
- ins: 밑줄 글자 태그
- del: 가운데 줄이 그어진 글자 태그

**여기서 HTML/1-8.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

## 테이블 태그 - 기본

- tr: 표 내부의 행 태그, table row
- th: 행 내부의 제목 셀 태그, table header
- td: 행 내부의 일반 셀 태그, table data
- thead, tbody, tfoot: 시멘틱 태그

**여기서 HTML/1-9.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

## 테이블 태그 - 속성

- table 태그의 속성
    - border: 표의 테두리 두께를 지정
    - width: 표의 너비를 지정

- th 태그와 td 태그 속성
    - rowspan: 셀의 행 확장 범위 지정
    - colspan: 셀의 컬럼 확장 범위 지정

**여기서 HTML/1-10.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

## 공간 분할 태그

- div: block 형식으로 공간을 분할
    - 쌓아 올려지는 형식
- span: inline 형식으로 공간을 분할
    - 한 줄 안에 차례차례 위치하는 형식

| Block 형식 태그 | Inline 형식 태그 |
| --- | --- |
| div, h1~h6, p, 목록(ol, ul), 테이블, form 태그 | span, a, input, 글자 형식 태그들 |

**여기서 HTML/1-11.html 코드를 참고해보세요!**

**코드를 Live Server로 확인해보세요!**

### Reference

- [https://github.com/kdkcom1234/git2021/tree/master/1-html-css/example/ch01](https://github.com/kdkcom1234/git2021/tree/master/1-html-css/example/ch01)
- [모던 웹을 위한 HTML5+CSS3 바이블(3판)윤인성 | 한빛미디어](http://www.kyobobook.co.kr/product/detailViewKor.laf?mallGb=KOR&ejkGb=KOR&barcode=9791162241585)
- **HTML5 and CSS Fundamentals, edX(W3Cx)**
