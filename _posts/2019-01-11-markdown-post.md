---
layout: post
title: Markdown 공부
subtitle: markdown
tags: [post, markdown, 마크다운, 공부]
comments: true
image: /img/Markdown-mark.svg
---
  
# 마크다운이란?
  
___
  
`마크다운(markdown)은 일반 텍스트 문서의 양식을 편집하는 문법이다[1](http://daringfireball.net/projects/markdown/).`  
평소 github에서 자주 보이던 readme.md 파일에 md포맷이 바로 마크다운 확장자이다.  
마크다운을 이용하여 작성하면 쉽게 html형태로 변환이 가능하고, 복잡한 포맷이 없어 누구나 쉽게 작성이 가능하다.
  
___
  
  
# 마크다운 장단점
  
___
  
## 마크다운 장점
- 작성에 특별한 포맷이 필요하지 않다.
- 관리가 쉽다.
- 다양한 곳에서 md 포맷을 지원한다.
  
## 마크다운 단점
- 표준이 없다.
- 멀티미디어 처리가 불편한다.
  
___
  
  
# 마크다운 문법
  
___
  
## 제목
html에서 `<h1>` ~ `<h5>`를 표현한다.
```markdown
# <h1>
## <h2>
### <h3>
#### <h4>
##### <h5>
```
# h1
## h2
### h3
#### h4
##### h5
  
___
  
## 강조
html 코드에로서 `<em>`, `<strong>`, `<del>`, `<u>` 태그를 나타낼 수 있다.
```markdown
이텔릭체(`<em>`) 태그는 *별표*, _언더바_ 사용
강조(`<strong>`) 태그는  **별표 두번**, __언더바 두번__ 사용
_**강조된 이텔릭체**_ 도 표현 가능함

취소선(`<del>`) 태그는 ~~물결표~~ 사용
밑줄(`<u></u>`) 태그는 <u>밑줄<u> 사용

```
이텔릭체(`<em>`) 태그는 *별표*, _언더바_ 사용  
강조(`<strong>`) 태그는  **별표 두번**, __언더바 두번__ 사용  
_**강조된 이텔릭체**_ 도 표현 가능함  
취소선(`<del>`) 태그는 ~~물결표~~ 사용  
밑줄(`<u></u>`) 태그는 <u>밑줄<u> 사용  
  
___
  
## 목록
html 코드에 `<ol>`, `<ul>` 태그를 나타낼 수 있다.
```markdown
1. 순서가 있는 목록
1. 순서가 있는 목록
    - 순서가 없는 서브 목록
    - 순서가 없는 서브 목록
1. 순서가 있는 목록
    1. 순서가 있는 서브 목록
    1. 순서가 있는 서브 목록
1. 순서가 있는 목록

- 순서가 없는 목록에 사용 가능한 기호
  - 대쉬
  * 별표
  + 더하기
  ```
1. 순서가 있는 목록
1. 순서가 있는 목록
    - 순서가 없는 서브 목록
    - 순서가 없는 서브 목록
1. 순서가 있는 목록
    1. 순서가 있는 서브 목록
    1. 순서가 있는 서브 목록
1. 순서가 있는 목록

- 순서가 없는 목록에 사용 가능한 기호
  - 대쉬
  * 별표
  + 더하기
  
___
  
## 링크
```markdown
html 코드에 <a> 태그를 나타낼 수 있다.
[표시되는 텍스트](링크 title 속성 내용) 으로 표현할 수 있다.
이때 title 속성 내용은 optional 입니다.

[구글](https://google.com)
  
[네이버](https://naver.com "네이버 입니다!")
  
[상대 경로(home)](../../)
  
참조링크를 아래와 같이 사용 할 수도 있다.
  
[jaehyun lim 의 GitHub]
  
[GitHub][1]

[1]: https://github.com
  
[jaehyun lim 의 GitHub]: https://github.com/vljh246v "jaehyun의 github!"
  

아래와 같이 url을 표현할 경우 자동으로 `<a>`태그로 인식한다.

네이버 : <https://naver.com>
```
  
[구글](https://google.com)
  
[네이버](https://naver.com "네이버 입니다!")
  
[상대 경로(home)](../../)
  
참조링크를 아래와 같이 사용 할 수도 있다.
  
[jaehyun lim 의 GitHub]
  
[GitHub][1]

[1]: https://github.com
  
[jaehyun lim 의 GitHub]: https://github.com/vljh246v "jaehyun의 github!"
  

아래와 같이 url을 표현할 경우 자동으로 `<a>`태그로 인식한다.
네이버 : <https://naver.com>
  
___
  
## 이미지
html 코드에 `<img>` 태그를 나타낼 수 있다.
```markdown
![alt 속성 내용](링크 title 속성 내용) 으로 표현할 수 있다.
링크와 비슷하지만 맨 앞에 ! 기호가 붙음
이때 title 속성 내용은 optional 입니다.

![사진이 안보입니다. 크리스마스-1](https://github.com/vljh246v/vljh246v.github.io/blob/master/img/test-img1.jpg?raw=true  "크리스마스1")

![사진이 안보입니다. 크리스마스-2][img2]

[img2]: https://github.com/vljh246v/vljh246v.github.io/blob/master/img/test-img2.jpg?raw=true "크리스마스2"
```
![사진이 안보입니다. 크리스마스-1](https://github.com/vljh246v/vljh246v.github.io/blob/master/img/test-img1.jpg?raw=true  "크리스마스1")

![사진이 안보입니다. 크리스마스-2][img2]

[img2]: https://github.com/vljh246v/vljh246v.github.io/blob/master/img/test-img2.jpg?raw=true "크리스마스2"
  
___
  
## 이미지 + 링크
html 코드에
```html
<a href='...' >
    <img src='...' alt='...'>
</a>
```
태그를 나타낼 수 있다.
```markdown
[![GitHub](https://raw.githubusercontent.com/vljh246v/vljh246v.github.io/master/img/avatar-icon.png)](https://github.com)
```
[![GitHub](https://raw.githubusercontent.com/vljh246v/vljh246v.github.io/master/img/avatar-icon.png)](https://github.com)
  
___
  
## 인용문
html 코드에 `<blockquote>` 태그를 나타낼 수있다.
```markdown
> 이것은
> > 인용문
> > > 입니다.
```
> 이것은
> > 인용문
> > > 입니다.
  
___
  
## 단일 라인 코드 강조
html 코드에 `<code>` 태그를 나타낼 수있다.
```markdown
`String tempStr = "코드를 강조하라!"`
```
`String tempStr = "코드를 강조하라!"`
  
___
  
## 블럭 라인 코드 강조
html 코드에 
```html
<pre>
    <code>...</code>
</pre>
```
태그를 나타낼 수있다.
\``` 기호를 3번 입력 후 표현하고 싶은 언어를 적고  
\``` 기호를 다시 3번 입력하여 닫아준다.  

```markdown

\```(소스코드 종류)`
    xxx xxx xx
\```

```

```html
<a href="https://www.google.co.kr/">구글</a>
```

```css
.list > li {
  position: absolute;
}
```

```javascript
function foo() {
    var tempStr = 'Hello, World'
}
```

```bash
$ vim ./~mylist
```

```python
s = "Hello, Python
print s
```
