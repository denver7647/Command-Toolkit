# MARKDOWN

<br>

# 목차
1. [마크다운(MARKDOWN)이란](#마크다운markdown이란)

2. 마크다운 문법
    - [Headers 헤더](#headers-헤더)
    - [Horizontal Rules 수평선](#horizontal-rules-수평선)
    - [Emphasis 강조](#emphasis-강조)
    - [Blockquotes 인용](#blockquotes-인용)
    - [Backslash Escapes](#backslash-escapes)
    - [image 이미지](#image-이미지)
    - [code blocks 코드 블럭](#code-blocks-코드-블럭)
    - [check list 체크리스트](#check-list-체크리스트)
    - [Table 테이블](#table-테이블)
3. 기타
    - [이모지](#이모지)
    - [color 색상](#color-색상)
    - [사이트 모음](#사이트-모음)

<br><br>

# 마크다운(MarkDown)이란

마크다운(MarkDown)은 문서를 읽고, 쓰고, 편집하기 쉬운 목적으로 만들어진 문서 작성을 위한 형식으로 문법이 간결하고 HTML삽입이 가능하다.

<br>

**[마크다운 장점]**
1. 문법이 간결하고 쉽다.
2. 관리가 간편하다.
3. 지원 가능 플랫폼 및 프로그램이 다양하다.(대부분 환경에서 지원가능)
4. 텍스트 형식으로 용량이 비교적 적다.

<br>

**[마크다운 단점]**
1. 모든 HTML의 문법을 대신하진 못한다.
2. 표준이 없어 플랫폼에 따라 생성물이 조금씩 다르다.

<br><br>

# 마크다운 (MarkDown) 문법

<br>

## **Headers 헤더**
\#로 시작하는 텍스트로 h1, h2, h3, h4, h5, h6의 태그를 표현할 수 있습니다.

``` MARKDOWN
# This is H1
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6

```

# This is H1
## This is H2
### This is H3
#### This is H4
##### This is H5
###### This is H6


``` MARKDOWN
This is H1
===

This is H2
---
```

This is H1
===

This is H2
---

<br><br>

## **Horizontal Rules 수평선**

-, _ 또는 *을 3개 이상 작성하여 표현 <br>
-의 경우 header로 인식할 수 있으니 주의!!!

``` MARKDOWN

* * *
***
*****
- - -
-------------------

```

* * *
***
*****
- - -
-------------------
<br> <br>

## **Emphasis 강조**

기울여 쓰기, 두껍게 쓰기 , 취소선 등 표현

``` MARKDOWN
_italic 기울인 글씨_ 
*italic 기울인 글씨*

__bold 굵게, 굵은 글씨__ 
**bold 굵게, 굵은 글씨**

~~Strikethrough 텍스트~~

<U>Underscore 밑줄</U>

_**혼합하여** <U>다양하게</U> ~~사용하기~~_

```

_italic 기울인 글씨_ <br>
*italic 기울인 글씨*

__bold 굵게, 굵은 글씨__ <br>
**bold 굵게, 굵은 글씨**

~~Strikethrough 텍스트~~

<U>Underscore 밑줄</U>

_**혼합하여** <U>다양하게</U> ~~사용하기~~_

<br><br>

## **Blockquotes 인용**
\> 으로 시작하는 텍스트로 인용의 목적으로 사용 <br>
※**인용**이란 의미를 명확하게 하거나 인용되는 글의 주장을 뒷받침할 때,<br>     또는 인용되는 글에 대한 직접적인 정보를 제공하는 경우를 뜻함.

``` MARKDOWN
0 depth
>1 depth
>>2 depth
>>>3 depth
```

0 depth
>1 depth
>>2 depth
>>>3 depth

<br><br>
## **Lists 목록**

### **순서가 없는 목록**

\* , + , - 를 이용하여 순서가 없는 목록 생성 가능 <br>
들여쓰기를 통하여 표현

``` MARKDOWN
* depth
    * depth
    * depth
        * depth
        * depth
        * depth

+ depth
    + depth
    + depth
        + depth
        + depth
        + depth

- depth
    - depth
    - depth
        - depth
        - depth
        - depth
```

* depth
    * depth
    * depth
        * depth
        * depth
        * depth

+ depth
    + depth
    + depth
        + depth
        + depth
        + depth

- depth
    - depth
    - depth
        - depth
        - depth
        - depth

### **순서가 있는 목록**

``` MARKDOWN
1. depth
    1. depth
    2. depth
        1. depth
        1. depth
        1. depth
2. depth
    1. depth
    2. depth
        1. depth
        1. depth
        1. depth
```

1. depth
    1. depth
    2. depth
        1. depth
        1. depth
        1. depth
2. depth
    1. depth
    2. depth
        1. depth
        1. depth
        1. depth

### **혼합 리스트**

``` MARKDOWN
1. depth
    - depth
    - depth
        + depth
        + depth
        + depth
2. depth
    - depth
    - depth
        + depth
        + depth
        + depth
```

1. depth
    - depth
    - depth
        + depth
        + depth
        + depth
2. depth
    - depth
    - depth
        + depth
        + depth
        + depth

<br><br>

## **Backslash Escapes**

특수문자를 표현할때, 문자 앞에 \\를 넣고 특수문자 이용

``` MARKDOWN
* 특수문자 출력안됨
- 특수문자 출력안됨

\* 특수문자 출력

\- 특수문자 출력
```

* 특수문자 출력안됨
- 특수문자 출력안됨

\* 특수문자 출력

\- 특수문자 출력

<br><br>

## **image 이미지** 

이미지 앞에 \!를 붙여서 표현 <br>
인라인 이미지 표현 : \!\[alt text\](/test.png) <br>
링크 이미지 표현 : \!\[alt text\](image_URL) <br>
사이즈 컨트롤 기존 img 태그 이용 : \<img width="OOOpx" height="OOOpx"\>\</img\>

``` MARKDOWN
![텍스트](이미지파일경로.jpg "이미지이름") 
![텍스트](이미지파일URL "이미지이름")

[ ![텍스트](이미지URL) ]( 링크URL )

[![텍스트](https://t1.daumcdn.net/cfile/tistory/2444873B57E257821F)](https://unity3d.com/kr)

<img src="https://i1.sndcdn.com/avatars-000639959556-jhitcq-t500x500.jpg" width="200" height="200" />

<a href="#">
	<img src="https://github.com/images/markdown_syntax.jpg" width="100px" alt="sample image">
</a>
```
[![텍스트](https://t1.daumcdn.net/cfile/tistory/2444873B57E257821F)](https://unity3d.com/kr)

<img src="https://i1.sndcdn.com/avatars-000639959556-jhitcq-t500x500.jpg" width="200" height="200" />

<a href="#">
	<img src="https://i1.sndcdn.com/avatars-000639959556-jhitcq-t500x500.jpg" width="100px" alt="sample image">
</a>

<br><br>
## **Links (Anchor) 링크**

``` MARKDOWN
[Google](http://www.google.com "구글")

[Naver](http://www.naver.com "네이버")

[Github](http://www.github.com "깃허브")

[MyGithub](https://github.com/denver7647 "나의 깃허브")

구글 www.google.com

네이버 <www.naver.com>


```

[Google](http://www.google.com "구글")

[Naver](http://www.naver.com "네이버")

[Github](http://www.github.com "깃허브")

[MyGithub](https://github.com/denver7647 "나의 깃허브")

구글 www.google.com

네이버 <www.naver.com>

<br><br>

### **내부(해시) 링크**
\[보여지는 내용](#이동할 헤드(제목))괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성

``` MARKDOWN
[1. Headers 헤더](#1-headers-헤더)

[2. Emphasis 강조](#2-emphasis-강조)

[3. Blockquotes 인용](#3-blockquotes-인용)
```

[1. Headers 헤더](#1-headers-헤더)

[2. Emphasis 강조](#2-emphasis-강조)

[3. Blockquotes 인용](#3-blockquotes-인용)

<br><br>

## **code blocks 코드 블럭**
간단한 코드는 코드 앞뒤로 **\`** 를 넣어서 표현. <br>
또는 **\``` , \~~~** 넣어서 표현 <br>
**\```** 옆에 JAVA , MARKDOWN 등 표시 가능

``` MARKDOWN
``` javascript
function test() {
 console.log("Hello world");
}
\```
```

``` javascript
function test() {
 console.log("Hello world");
}
```

<br><br> 

## **check list 체크리스트**

줄 앞에 - [x]를 써서 완료된 리스트 표시. <br>
줄 앞에 - [ ]를 써서 미완료된 리스트 표시. <br>
체크 안에서 강조 외에 여러 기능을 사용할 수 있습니다. <br>

``` MARKDOWN
- [x] this is a complete item
- [ ] this is an incomplete item
```
- [x] this is a complete item
- [ ] this is an incomplete item


<br><br>

## **Table 테이블**
헤더와 셀을 구분할 때 3개 이상의 **- (hyphen/dash)** 기호가 필요합니다. <br>
헤더 셀을 구분하면서 **: (Colons)** 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다. <br>
가장 좌측과 가장 우측에 있는 **| (vertical bar)** 기호는 생략 가능합니다. <br>

``` MARKDOWN
테이블 생성

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12
```


헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8
셀9|셀10|셀11|셀12

``` MARKDOWN
테이블 정렬

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9
```

헤더1|헤더2|헤더3
:---|:---:|---:
Left|Center|Right
1|2|3
4|5|6
7|8|9

<br><br>

# **기타**

<br>

## **이모지**
**\: :** 사이에 이모지 관련 텍스트를 넣으면 사용 가능 <br>

``` MARKDOWN
:smirk: : smirk <br>
:heart_eyes: : heart_eyes <br>
:kissing_heart: : kissing_heart <br>
```

:smirk: : smirk <br>
:heart_eyes: : heart_eyes <br>
:kissing_heart: : kissing_heart <br>

:arrow_right: [이모지 사이트 링크](https://www.webfx.com/tools/emoji-cheat-sheet/ "이모지") :arrow_left:

<br><br>

## **color 색상**

``` MARKDOWN
font-color

<span style="color:red"> red </span> 
<span style="color:#ffd33d"> yellow </span> 
<span style="color:blue"> blue </span> 
<span style="color:brown"> brown </span> 
<span style="color:orange"> orange </span> 
<span style="color:green"> green </span> 
<span style="color:violet"> violet </span> 
<span style="color:yellowgreen"> yellowgreen </span> 
<span style="color:blueviolet"> blueviolet </span> 
<span style="color:gray"> gray</span> 
<span style="color:indigo"> indigo </span> 
```

<span style="color:red"> red </span> <br>
<span style="color:#ffd33d"> yellow </span> <br>
<span style="color:blue"> blue </span> <br>
<span style="color:brown"> brown </span> <br>
<span style="color:orange"> orange </span> <br>
<span style="color:green"> green </span> <br>
<span style="color:violet"> violet </span> <br>
<span style="color:yellowgreen"> yellowgreen </span> <br>
<span style="color:blueviolet"> blueviolet </span> <br>
<span style="color:gray"> gray</span> <br>
<span style="color:indigo"> indigo </span> <br>



``` MARKDOWN
background color

<span style="background-color:#fff5b1"> 노란형광펜 </span>
<span style="background-color:#FFE6E6"> 빨강형광펜 </span>
<span style="background-color:#E6E6FA"> 보라형광펜 </span>
<span style="background-color:#C0FFFF"> 파랑형광펜 </span>
<span style="background-color:#FFFFF0"> 노란형광펜 </span>
<span style="background-color:#F5F5F5"> 회색형광펜 </span>
<span style="background-color:#DCFFE4"> 초록형광펜 </span>
```

<span style="background-color:#fff5b1"> 노란형광펜 </span> <br>
<span style="background-color:#FFE6E6"> 빨강형광펜 </span> <br>
<span style="background-color:#E6E6FA"> 보라형광펜 </span> <br>
<span style="background-color:#C0FFFF"> 파랑형광펜 </span> <br>
<span style="background-color:#FFFFF0"> 노란형광펜 </span> <br>
<span style="background-color:#F5F5F5"> 회색형광펜 </span> <br>
<span style="background-color:#DCFFE4"> 초록형광펜 </span> <br>

<br><br>

## 사이트 모음
<br>

- markdown 미리보기
	- [stackedit](https://stackedit.io/app#  "stackedit")
 	- [jbt.github.io](https://jbt.github.io/markdown-editor/  "jbt.github.io")

- 이모지 
	- [webfx](https://www.webfx.com/tools/emoji-cheat-sheet/ "webfx")
