# 마크다운

## 마크다운이란?

마크다운은 텍스트 기반의 마크업 언어            
문법이 쉽고 간단한 것이 특징            
HTML과 리치 텍스트 드으이 서식문서로 쉽게 변환 가능             
특수기호와 문자 등을 이용한 문법으로 빠르고 간단하게 컨텐츠 작성 가능

## 마크다운 장점

1. 간단한고 쉬운 문법
2. 확장성이 좋다
3. 텍스트로 저장되기 때문에 용량이 적음
4. 텍스트로 저장되기 때문에 검색이 쉬움
5. 지원하느 프로그램 및 플랫폼이 다양

## 마크다운 단점

1. 표준이 없고 도구에 따라 변환 방식이나 생성물이 다름
2. 뷰어의 속도가 느림
3. 모든 HTML 마크업을 대체하지 못함

## 마크다운의 문법

`<h1>` 부터 `<h6>` 까지 `#` 을 이용하여 제목을 나타낼 수 있다.

```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

# h1
## h2
### h3
#### h4
##### h5
###### h6

## 인용문

`>` 블록인용 문자를 사용한다

### 단일 블록 인용문
> This is a single blockqute.

### 복수 블록 인용문

> This is nested blockqute.
> > This is nested blockqute.
> > > This is nested blockqute.

## 목록
`<ol>` , `<ul>` 태그를 나타낸다

### 순서 있는 목록(ol)
순서 있는 목록은 숫자와 점을 사용한다.
1. 첫번째
2. 두번째
3. 세번째

### 순서 없는 목록(ul)
글머리 기호 : *, +, - 를 지원한다

* 별표
+ 더하기
- 뺴기

### 목록 섞어서 사용하기
띄어쓰기 3번을 사용하면 됨           

~~~markdown
1. ordered list
   * unordered list
2. ordered list
   1. sub ordered list
   2. sub ordered list
- 순서가 필요하지 않는 목록에 사용 가능한 기호
   1. 숫자
      * 별표
      + 더하기
      - 대쉬
~~~

> output :
1. ordered list
   * unordered list
2. ordered list
   1. sub ordered list
   2. sub ordered list
- 순서가 필요하지 않는 목록에 사용 가능한 기호
   1. 숫자
      * 별표
      + 더하기
      - 대쉬

## 강조
```markdown
*Italic : single 별표*  
_Italic : single 밑줄_  
**Bold: double 별표**   
__Bold : double 밑줄__  
**Bold and _Italic_** and normal        
<u>Underline : user </u>     
~~LineThrough: double wavy~~    
```
> output
*Italic : single 별표*  
_Italic : single 밑줄_  
**Bold: double 별표**   
__Bold : double 밑줄__  
**Bold and _Italic_** and normal        
<u>Underline : user </u>     
~~LineThrough: double wavy~~    

## 링크
`<a>` 태그를 나타낸다.

### 링크 기본 문법

`[링크 설명]` `(url)` 방식으로 표현하여 `url` 을 `[Keyword]` 로 표현 할 수 있다.
```markdown
1. [Google](https://google.com)
2. [Naver](https://naver.com "이곳에 작성하는 링크 설명은 사용자에게 보이지 않음")
3. [로컬 링크](../)
4. [Github][1]
[1] : https://github.com
```

> output
1. [Google](https://google.com)
2. [Naver](https://naver.com "이곳에 작성하는 링크 설명은 사용자에게 보이지 않음")
3. [로컬 링크](../)
4. [Github][1]          
[1] : https://github.com

### 참조 링크
문서 안에 [참조 링크]를 사용할 수 있다.         
[참조 링크] : https://github.com

### 자동 연결

일반 URL이나 이메일 주소, 또는 꺾쇠 괄호(< >)안의 URL은 자동으로 링크를 생성한다.

```markdown
* 구글 홈페이지 : https://google.com
* 외부링크: <http://example.com>
* 이메일링크:  <gibeom2002@gmail.com>
```

>output
* 구글 홈페이지 : https://google.com
* 외부링크: <http://example.com>
* 이메일링크:  <gibeom2002@gmail.com>

## 줄바꿈

```markdown
마크다운에서는 엔터키 대신  
띄어쓰기 두번을 사용해야 한다.

글을 쓰다가 줄바꿈을 하고 싶을 경우  
엔터키로는 줄바꿈이 되지 않는다.  

줄바꿈 하고 싶은 문단의 마지막에  
띄어쓰기 두번을 사용하고 엔터키를 누른다.  

또는 쉽게 <br>태그를 사용할 수 있다.  
```

> output

마크다운에서는 엔터키 대신  
띄어쓰기 두번을 사용해야 한다.

글을 쓰다가 줄바꿈을 하고 싶을 경우  
엔터키로는 줄바꿈이 되지 않는다.  

줄바꿈 하고 싶은 문단의 마지막에  
띄어쓰기 두번을 사용하고 엔터키를 누른다.  

또는 쉽게 `<br>` 태그를 사용할 수 있다.  

## 수평선

마크다운 문서 작성 시 페이지 나누기 용도로 많이 사용한다. <hr/> 태그를 아래와 같이 표현 할 수 있다.

```markdown
___ (underscores x3)

--- (dash x3)

*** (asterisks x3)
```
> output
___
---
***

## 코드 블록

간단한 인라인 코드는 텍스트를 앞뒤로 ` `` ` 기호로 감싸면 됨  
` ``` ` 혹은 ` ~~~ ` 코드  
코드가 여러 줄인 경우, 줄 앞에 공백 네 칸을 추가하면 됨  
` ``` ` 앞에 언어를 지정해주는 syntax color가 적용됨

``` c
int main()
{
        printf("HELLO WORLD!\n");
        return 0;
}
```

## 이미지 넣기
```
:[Github Logo](./images/markdown_logo.jpg)
Format : :[이미지 alt명](url 링크)
```

>output

:[Github Logo](./images/markdown_logo.png)

## 테이블

```markdown
First Header | Second Header
------------ | -------------
Content1     | Content2
Content1-1   | Content2-2
```
>output

First Header | Second Header
------------ | -------------
Content1     | Content2
Content1-1   | Content2-2

## 체크 박스

```markdown
- [x] 체크박스 표시
- [ ] 체크박스 없음
```

>output

- [x] 체크박스 표시
- [ ] 체크박스 없음

## 이모지 및 배지

### 이모지 사용법
```markdown
Github supports emoji:
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:
```

>output

Github supports emoji:  
:+1: :sparkles: :camel: :tada:  
:rocket: :metal: :octocat:

> 자세한 것은 다음 링크 참조  
https://emoji.cheat-sheet.com

### 배지 사용법
```markdown
<img src="https://img.shields.io/badge/skill-c_lang-blue">
```

>output  
<img src="https://img.shields.io/badge/skill-c_lang-blue">  

> 자세한 것은 다음 링크 참조  
https://shields.io