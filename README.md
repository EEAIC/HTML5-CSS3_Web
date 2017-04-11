HTML5
===
# Basic

<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

* [HTML5](#html5)
* [Basic](#basic)
  * [Definition](#definition)
    * [HyperText Markup Lauguage](#hypertext-markup-lauguage)
    * [웹 브라우저와 편집기](#웹-브라우저와-편집기)
  * [문서 기본 구조](#문서-기본-구조)
  * [텍스트 태그](#텍스트-태그)
  * [이미지 태그](#이미지-태그)
  * [하이퍼링크](#하이퍼링크)
  * [폼](#폼)
  * [시맨틱 태그](#시맨틱-태그)
  * [멀티미디어 영역](#멀티미디어-영역)
  * [애니메이션](#애니메이션)
    * [변형](#변형)
      * [웹 문서 업로드](#웹-문서-업로드)
* [CSS](#css)
  * [Basic](#basic-1)
  * [Style](#style)
    * [스타일 형식](#스타일-형식)
    * [내부 스타일 시트](#내부-스타일-시트)
    * [외부 스타일 시트](#외부-스타일-시트)
    * [인라인 스타일](#인라인-스타일)
  * [주요 선택자](#주요-선택자)
    * [전체 선택자](#전체-선택자)
    * [태그 선택자](#태그-선택자)
  * [캐스캐이딩 스타일 시트](#캐스캐이딩-스타일-시트)
  * [CSS 모듈](#css-모듈)
  * [텍스트 스타일](#텍스트-스타일)
    * [font-family](#font-family)
    * [@font-face](#font-face)
    * [color 속성](#color-속성)
  * [문단 스타일](#문단-스타일)
  * [색상 표기법](#색상-표기법)
  * [배경](#배경)
    * [그라데이션](#그라데이션)
  * [박스 모델](#박스-모델)
    * [테두리](#테두리)
  * [CSS 포지셔닝](#css-포지셔닝)
    * [다단으로 편집하기](#다단으로-편집하기)
  * [표 스타일](#표-스타일)
  * [CSS3 선택자](#css3-선택자)
    * [연결 선택자](#연결-선택자)
    * [가상 클래스](#가상-클래스)

<!-- tocstop -->




## Definition
### HyperText Markup Lauguage
  * HyperText
    * 링크를 클릭해 다른 문서나 사이트로 이동
  * Markup
    * tag를 사용해 어느부분이 제목이고 본문인지 사진이고 링크인지 표시
  * 웹 편집기(web editor) = 웹 문서 작성
  * 웹 브라우저(web browser) = 웹 문서 보는 프로그램
* HTML5 = 웹 표준
  * 공식명칭은 'HTML'
### 웹 브라우저와 편집기
* 브라우저
  * 크롬
  * 파이어폭스
  * 인터넷 익스플로퍼
  * 엣지
* 편집기
  * 텍스트 편집기
  * 웹 편집기
  * IDE
  * 웹 기반 코드 편집기

## 문서 기본 구조

* `<!doctype html>` or `<!doctype html>`
  * Html 문서이고 버전임을 명시
* `<html>`
  * 실제 문서 정보와 내용이 시작되고 끝나는 것을 표시하는 태그
  * `<html lang="ko">`
    * 사용할 언어 지정
* `<head>`
  * 웹 브라우저 화면상에는 보이지 않음
  * `<title>`
    * 제목 표시줄에 표시되는 내용
  * `<meta>`
    * 문자 인코딩 방법 및 요약 정보
  * `<meta charset="utf-8">`
* `<body>`
  * 실제 표시될 내용 부분

## 텍스트 태그

* `<hn>`
  * 제목을 표시할 때 사용하는 태그
  * n이 작을수록 글잨 크기가 큼
* `<p>`
    * 텍스트 단락
* `<br>`
    * 줄 바꾸기
    * 닫는 태그 없음
* `<blockquote>`
    * 인용문 넣기
    * 들여 쓰여짐
* `<hr>`
    * 수평줄 생김
    * 주제가 바뀔 때 전환 효과
    * 닫는 태그 없음
* `<pre>`
    * 소스에 표시한 공백 그대로 표시
* `<strong>, <b>`
    * `<strong>`
      * 중요한 내용
    * `<b>`
      * 단순히 굵게
* `<em>, <i>`
   * `<em>`
      * 특정 부분 강조
   * `<i>`
      * 단순히 이탤릭체
* `<q>`
    * 인용 내용 앞뒤에 (" ") 추가됨
    * 줄바꿈 없이 한줄에 인용 표시
* `<mark>`
    * 형광펜 효과
* `<span>, <div>`
    * CSS를 부분적으로 적용
    * `<span>`
      * 줄 안에서 묶기
    * `<div>`
      * 블럭으로 묶기
* `<ruby><rt>`
    * `<rt>`
      * 주석 표시      
* `<ui>, <li>`
    * 순서 없는 목록
* `<oi>, <li>`
    * 순서 있는 목록
    * `type="a"`
    * `start="1"`
    * `reserved`
* `<dl>,<dt>,<dd>`
    * 설명 목록
    * `<dt>`
      * 제목
    * `<dd>`
      * 내용
* `<table>, <tr>, <td>, <th>`
    * 표 만들기
    * `<caption>`
      * 표 이름
      * 이름은 하나만 가능
      * 중앙에 정렬
    * `<tr>`
      * 행
    * `<td>`
      * 셀
    * `<th>`
      * 제목이 있는 셀
    * `border="1"`
      * 표 테두리
* `<figure>`
    * `<figcaption>`
      * 대상에 이름 설정
      * 중앙에 정렬되지 않음
* `colspan="3", rowspan="3"`
    * `colspan="3"`
      * 행 합치기
    * `rowspan="3"`
      * 열 합치기
* `<thead>, <tbody>, <tfoot>`
    * 표 구조 정의
    * `<thead>`
      * 표 안에서의 제목 정의
    * `<tbody>`
      * 표 안에서의 내용 정의
    * `<tfoot>`  
      * 표 안에서의 요약 정의
    *  `<tbody>` 와 `<tfoot>` 은 순서 상관 없음
* `<col>, <colgroup>`
    * `<tr>, <td>` 전에 사용
    * 묶는 열의 개수 만큼 `<col>` 사용
    * `<col>`
      * 한 열의 모든 셀에 같은 스타일 적용
      * `span="2"`
        * 여러 열 묶기
      * 닫는 태그 없음

## 이미지 태그

* `<img src="경로"`>
  * 이미지 삽입
  * `alt="홈으로 가기"`
    * 이미지를 설명하는 대체 텍스트
    * 이미지 표시 불가시 표시
    * 화면 낭독기가 읽음
  * `width="숫자", height="숫자"`
    * 이미지 크기 조정
    * 이미지 용량은 그대로

## 하이퍼링크

* 외부 사이트나 외부 페이지로 연결
* `<a href="링크할 주소"> 텍스트나 이미지태그`
  * `target="_blank"`
    * 링크 내용이 새 창이나 새 탭에서 열림
  * 앵커
    * `<태그 id="앵커"> 텍스트 또는 이미지태그`
      `<a href="#앵커"> 텍스트 또는 이미지태그`
    * 한 페이지 안에서 이동하기
* 이미지맵
  * 한 이미지 안에 여러 링크 만들기
  * `<img src="경로 또는 주소" usemap="#맵이름">`
  * `<map name="맵이름">`
  * `<area shape="rect" coords="10,10,160,200 href="링크할 주소">`
    * `shape="rect"`
    * `coords="10,10,160,200"`

## 폼

* 웹 사이트로 정보를 보낼 수 있는 요소들
* 정보를 저장 및 검색 또는 수정
* 사용자 정보를 처리하는 것은 ASP나 PHP 같은 서버 프로그래밍
* `<form method="post">`
  * `method="get"`
    * 입력한 부분이 주소표시줄에 나타남
    * 4096byte의 길이 제한
  * `method="post"`
    * 입력한 내용이 드러나지 않음
    * 길이 제한 없음
  * `action="search.php"`
    * 폼 안의 내용을 처리하는 서버 상의 프로그램
* `<label>`
  * 입력 필드 옆에 표시 되는 부분
  * 폼 전체를 묶어서 사용하거나 폼과 연결하여 사용 가능
    * `<label for="user-id">`
* `<fieldset>`
* 폼 요소를 그룹으로 묶는 태그
  * `<legend>`
  * 그룹으로 묶는 구역에 제목을 붙이는 태그
* `<input type="유형">`
  * 사용자가 내용을 입력하는 부분
  * `type="hidden"`
    * 화면 상에는 보이지 않음
    * 서버로 함께 전송되는 요소
  * `type="password"`
    * 비밀번호 입력란
  * `type="text"`
    * 한 줄짜리 텍스트 입력 필드
    * 주로 아이디나 이름, 주소 등 텍스트 입력
  * `name="이름"`
    * 텍스트 필드를 구별
  * `size="5"`  
    * 텍스트 필드의 길이를 지정
  * `value="내용"`  
    * 텍스트 필드 부분에 표시될 내용
    * 패스워드 필드에는 없음
  * `maxlength="50"`
    * 입력할 수 있는 최대 문자 개수
  * `type="search"`
    * 검색 필드
    * 검색어 삭제 쉬움
    * 주로 모바일에서 지원
  * `type="email"`
    * 메일 주소 형식 자동 체크
    * 메일 주소 입력 필드
  * `type="url"`
    * 사이트 형식 자동 체크
  * `type="tel"`
    * 전화번호 입력
  * `type="radio"`
    * 여러 항목중 하나만 선택
    * `name="이름"`
      * 모두 같아야 함
    * `value="내용"`
      * 서버에 전달될 값
  * `type="checkbox"`
    * 여러 항목 중 둘 이상 선택
    * `name="이름"`
      * 모두 달라야 함
    * `value="내용"`
      * 서버에 전달될 값
  * `type="submit"`
    * 폼 전송
    * 입력 내용을 서버로 전송
    * 사용자 입력 내용 전부 삭제
  * `type="reset"`
    * 사용자 입력 내용 전부 삭제
  * `type="image"`
    * submit 버튼 대신 이미지 삽입
  * `autofocus`
    * 원하는 폼 요소에 마우스 커서 표시
  * `placeholder="하이픈없이 입력"`
    * 입력란에 표시하는 힌트로, 필드를 클릭하면 사라짐
  * `readonly`
    * 폼 형식
    * 입력하지 못함
  * `required`
    * 필수 필드 체크
  * `min="10", max="100"`
    * 최소값, 최대값
    * 태그 유형이 date, datetime, datetime-local, month, week, time, number, range일 경우에만 사용
  * `step="2"`
    * 허용된 범위 내의 숫자의 일정한 간격
    * 태그 유형이 date, datetime, datetime-local, month, week, time, number, range일 경우에만 사용
  * `<select>`
    * 여러 옵션 중 하나 이상을 선택 가능
    * `<option>`
      * 드롭다운 목록
    * `<optgroup>`
      * 여러 항목을 그룹으로 묶음
  * `<datalist id="choices">`
    * **input** 의 **list** 속성에 **id** 를 입력하여 값이 자동으로 입력되게 할 수 있음
    * 사용자가 직접 텍스트 필드 입력 가능
  * `<textarea>`
    * 여러 줄의 텍스트 입력
    * `cols="100", rows="100"`
      * 가로 너비 지정 가능
  * `<button>`
    * 다양한 형태의 버튼 삽입
* `<output>`   
  * 계산 결과를 브라우저에 표시
  * 웹 브라우저가 계산의 결과값인 것을 정확히 인지
* `<progress>`
  * 작업 진행 상태를 브라우저에 표시
  * `max="60"`
  * `value="50"`
    * 작업의 진행의 현재 상태
* `<meter>`
  * 전체 크기 중 얼마나 차지하는지를 표시
  * `low="100", high="1024"`
  * `optimum="0.8"`
    * **optimum** 값이 **high** 값보다 크면 **value** 값이 클수록 좋고 **low** 보다 작으면 **value** 값이 작을수록 좋음

## 시맨틱 태그

* `<header>`
  * 사이트 전체의 제목 부분이 될 수도 있고, 본문의 제목 부분이 될 수도 있음
  * `<form>` 를 사용해 검색창을 넣거나 `<nav>` 태그를 사용해 사이트 메뉴를 넣음
* `<nav>`
  * 같은 사이트 안의 문서나 다른 사이트의 문서를 연결하는 링크를 나타냄
* `<section>`
  * 주제별 콘텐츠를 묶을 때 사용
* `<article>`
  * 웹 상의 실제 내용
  * 독립적으로 배포하거나 재사용하더라도 완전한 하나의 콘텐츠
* `<aside>`
  * 본문 내용에 영향을 미치지 않는 내용
* `<iframe src="삽입할 문서 주소" width=95% height="500">`
  * 문서 안에 외부 문서 삽입
* `<footer>`
  * 사이트의 제작자의 연락처 정보와 저작권 정보를 표시
* `<address>`
  * 제작자 정보와 연락처 정보
* `<div>`
  * 시각적 효과를 적용할 때 콘텐츠를 묶을 때 사용
* [html5shiv]("https://github.com/aFarkas/html5shiv")
  * IE8 이하 버전에서 사용
  * `<head>` 사이에 js 파일 삽입

## 멀티미디어 영역
* 외부 파일 삽입
  * `<object data="경로" type="유형" name="이름" width="너비" height="높이">`
    * 자바 애플릿이나 PDF, 플래시 무비 등 삽입
  * `<embed src="경로" type="유형" width="너비" height="높이">`
    * `<object>`를 지원 하지 않는 브라우저에서는 `<embed>` 사용
* 비디오 코덱
  * H.264/AVC
    * 고화질의 영상
    * .mp4 .mov 파일 등에서 사용
    * 유료 코덱이지만 온라인 사용시 무료
  * 오그 테오라(Ogg Theora)
    * 공개 코덱
    * 화질이 떨어짐
    * MS는 미지원
  * v8, v9
    * 오픈 소스로 공개한 코덱
    * 화질 좋고 무료
    * MS는 미지원
* 오디오 코덱
  * MPEG-1 AUDIO Layer3 (MP3 코덱)
    * 유료
    * .mp3 파일에서 사용
  * 오그 보비스(Ogg Vorbis)
    * 공개 코덱
    * .ogg 파일 형식에서 사용
    * 재생 플레이어가 적고 인코딩 시간이 더 걸린다는 단점
* `<audio src="오디오 파일 경로" controls>`
  * 배경 음악이나 효과음 등 오디오 재생
* `<video src="비디오 파일 경로" controls>`
  * `<video autoplay controls>`
    `<source src="비디오 파일 경로" type="video/mp4">`
* `<track kind="자막 종류" src="경로" srclang="언어" label="제목" default>`
  * WebVTT
    * 모든 브라우저에서 공식적으로 지원하는 자막 파일 형식
    * 자막 내용과 시간 정보를 함꼐 담고 있음

## 애니메이션
### 변형
* 2차원 변형
  * 수평 수직으로 웹 요소 변형
* 3차원 변형
  * 2차원에 원근감 추가
* `transform:translate(tx, ty)`
  * 지정한 방향으로 이동할 거리를 지정하면 해당 요소를 이동시킴
* `transform:scale(sx, sy)`
  * 지정한 크기만큼 요소를 확대/축소
* `transform:rotate(각도)`
  * 일반 각도나 래디안 값 사용
* `transform:rotate3d(rx, ry, rz)`
* `transform:skew(ax, ay)`
  * 요소를 지정한 각도만큼 비틀어 왜곡
* `transform-origin:<x축><y축><z축>`
  * 특정 지점을 변형의 기준으로 설정
* `perspective: <크기>`
  * 원근감을 갖게 함
  * 속성 값을 0보다 커야함
* `perspective-origin: <x축 값>`
* `transfom-style: preserve-3d`
  * 부모 요소에 적용한 3D 변형을 하위 요소에도 적용
*  `backface-visibility: visible`
  * `visible` 기본값
  * 요소의 뒷면을 표시할 것인지 결정
  





#### 웹 문서 업로드

* FTP 프로그램
  * 각종 파일을 서버로 업로드하거나 다운로드


CSS
===
Basic
---
## Style
* style: 자주 사용하는 글꼴이나 색상, 정렬 등 겉모습을 결정 짓는 내용들
* style sheet: 스타일을 한 군데 모아놓은 것
### 스타일 형식
* `p{text-align: center;}`
  * p: 선택자
  * text-align: 스타일 속성
  * centerg 속성 값
  * 속성 값이 여럿일 경우 세미콜론(;)으로 구분
* 스타일 주석
  * `/* */`
### 내부 스타일 시트
* `<head>` 태그 사이에서 정의
* `<style>`와 `</style>`사이에 작성
### 외부 스타일 시트
* 여러 웹 문서에서 사용할 스타일을 별도로 저장
* `<style>`없이`<link>`만 사용해 미리 만들어 놓은 외부 스타일 시트와 연결
* `rel="stylesheet"`
  * 연결하려는 문서의 속성
### 인라인 스타일
* 스타일 시트 사용하지 않고 스타일을 직접 대상에 표시
* `style="속성: 속성 값"`

## 주요 선택자
### 전체 선택자
* `p *{속성: 속성 값}`
  * 모든 하위 요소에 한꺼번에 스타일을 적용
### 태그 선택자
* `h1{스타일}`
  * 특정 태그를 사용한 모든 요소에 스타일이 적용됨
* 클래스 선택자
  * `.bluetext{ color: blue; }`
  * 문서 안에서 여러번 사용가능
  * `class = "bluetext"`
* id 선택자  
  * `#container{ margin: 0 auto;}`
  * 문서 안에서 한번만 사용
* 그룹 선택자
  * `h1,h2{text-align: center}`
## 캐스캐이딩 스타일 시트  
* 스타일 우선 순위
  * 스타일 규칙의 중요, 적용범위에 따라 결정
  * 위에서 아래로 적용
  * 인라인>id>클래스>태그
* 스타일 상속
  * 부모요소에서 자식요소로 상속
  * 모든 속성이 상속되는 것은 아님
  * 배경색은 상속되지 않음
* 사용자스타일 시트
  * 시스템에서 만든 스타일
  * 제어 불가
* 제작자스타일 시트
  * 웹 사이트를 만들 때 제작자가 만든 스타일
* 브라우저 스타일 시트

## CSS 모듈
* 속성 이름 앞에 접두사(prefix)를 붙여 브라우져별로 구분

|접두사|설명|
|:---:|:---:|
|-webkit-|웹키트 방식 브라우저용(사피리, 크롬 등)|
|-moz-|게코 방식 브라우저용(모질라, 파이어폭스 등)|
|-o-|오페라 브라우저|
|-ms-|마이크로소프트 인터넷 익스플로러|

* -prefix-free.js
  * 브라우저 벤더 접두사를 자동으로 붙여줌
  * `<script src="prefixfree.min.js"></script>`

## 텍스트 스타일
### font-family
* `body{font-family: "맑은 고딕", 돋움, 굴림}`  
* 속성은 상속됨
* space가 들어갈 경우 **""** 사용
### @font-face
* 웹 폰트(web-font): 웹 문서 안에 글꼴 정보도 함께 저장
* 제작가가 의도한 대로 텍스트를 표시할 수 있다.
  * 구글 웹 폰트
  * `@import url{http://fonts.googleapis/com/earlyaccess/nanumgothic.css}`
* `font-size: 20px`
    * `font-weight: 400`
      * 100~900
      * bold
    * `font-style: normal`
      * *italic*
### color 속성
* `color: <색상>`
* `text-decoration: underline`

|속성 값|설명|
|:---:|:---:|
|none| 밑줄을 표시하지 않습니다.|
|underline| 밑줄을 표시합니다.|
|overline| 영역 위로 선을 그립니다.|
|line-through| 영역을 가로지르는 선(취소 선)을 그립니다.|

* `text-shadow: <가로거리><세로거리><번짐 정도><색상>`
  * 가로거리 세로거리는 필수 속성
*  `white-space: pre-wrap`
  * 공백 처리 방법 지정
* `letter-spacing: <크기>`
* `word-spacing: <크기>`

## 문단 스타일
* `text-indent: <크기 or 백분율>`
  * 문단의 첫 글자 들여 쓰기
* `line-height: normal`
  * 문단의 줄 간격 지정
  * <숫자>와 <백분율>
* `line-style-type: none`
  * 순서없는 목록의 불릿 바꾸기
  * 순서 목록의 숫자 바꾸기
* `list-style-image: url('images/dot.png')`
  * 순서없는 목록의 불릿을 이미지로 바꾸는 속성
* `list-style-postion: inside`
  * 불릿이나 번호를 들여 쓰거나 내어쓸 수 있음
* `list-style: lower-alpha, inside`
  * 모든 속성을 한꺼번에 표시

## 색상 표기법  
* 16진수 표기법
  * `#ffff00`
* rgb/rgba 표기법
  * `color: rgba(255,0,0,.3)`
* hsl/hsla 표기법
  * `color: hsla(240,100%,50%,0.3)`
* 색상 이름 표기법
  * 기본 색상 16가지를 포함해 모두 216가지

## 배경
* `background-color: <색상>`
* `background-clip: <속성>`
  * 박스 모델 기준
* `background-image: url('파일경로')`
  * 배경 이미지 지정
* `background-repeat: repeat`
  * 배경 이미지 반복 여부 및 반복 방향 지정
* `background-size: auto`
  * contain
  * cover
* `background-position: <수평 위치><수직 위치>`
  * 배경 이미지를 반복하지 않고 배경 이미지를 표시할 위치 지정
* `background-attachment: scroll`
  * 배경 이미지를 고정하는 속성
* `background: url('images/bg3.jpg') no-repeat`
  * 배경 관련 속성을 줄여서 표기
  * 순서 상관 없음
### 그라데이션
* 구형 모던 브라우저에서는 브라우저 접두사를 붙여야 함
*
* `linear-gradient(<각도> to <방향>, blue, <색상 중지점>,  white)`
  * 방향
    * 끝 지점을 기준으로 'to' 키워드와 함께 사용
  * 각도
    * 그라데이션이 끝나는 각도
  * 색상 중지점
    * `white 30%`
    * 기본값: 가운데
* `radial-gradinet(<최종 모양> <크기> at <위치>, white yellow, red)`
  * 위치
    * 원의 중심 지점
    * 백분율이나 키워드
  * 크기
    * `closest-side`
    * `closest-corner`
    * `farthset-side`
    * `farthset-corner`
  * 색상 중지점
    * `red 40%`
    * 기본값: 50%
  * 그라데이션 반복
    * `repeating-linear-...`
    * '패턴'을 만들어 반복시킴
* [Gradient CSS Generator](http://www.cssmatic.com/gradient-generator)  

## 박스 모델
* 블록 레벨 요소
  * 요소의 너비가 100%
* 인라인 레벨 요소
  * 줄을 차지하지 않는 요소
* `width: 50%` `height: 100px`  
* `display: block`
  * 해당 요소를 블록 레벨로 지정
* `display: inline`
  * 해당 요소를 인라인 레벨로 지정
* `display: inline-block`
  * 요소를 인라인 레벨로 배치하면서 내용에는 블록 레벨 속성을 지정
* `display: none`
  * 요소를 표현하지 않음
  * 공간도 차지하지 않음
### 테두리  
* `border-style: solid`
  * 기본값이 none
* `border-width: 5px 10px 15px 20px`
  * top, right, bottom, left
  * 키워드
    * thin, medium, thick
  * 1개 지정
    * 네 방향 동일
  * 2개 지정
    * 위아래, 좌우
  * 3개 지정
    * top, right, bottom
    * left = right
  * 4개 지정
    * 각각
* `border-<방향>-color: <색상> `
    * `border-color: <색상>`
* `border: <속성>`
  * 테두리 스타일과 두꼐, 색상 등을 묶어 표기
  * 순서 상관없음
* `border-radius`
  * 박스 모서 부분을 둥글게 처리
  * `border-top-left-radius: 100px 50px`
    * 왼쪽 위 라운딩
  * `box-shadow: <수평 거리> <수직 거리> <흐림 정도> <번짐 정도> <색상>`
    * 수평 거리와 수직 거리는 필수, 기타 속성 값은 옵션
  * `padding-top: <크기> or <백분율>`
  * `margin-top: <크기> or <백분율>`

## CSS 포지셔닝
* 문서 요소를 적절히 배치하는 것
* `box-sizing: content-box`
  * 박스 모델의 너비 값 기준 지정
* `float: left`
  * 왼쪽이나 오른쪽에 떠 있게 만듦
* `clear: left`
  * float 속성을 무효화 시키는 속성
* `position: static`
  * 웹 문서 안에 요소들을 배치하기 위한 속성
  * `static`
    * 문서의 흐름대로 배치
  * `relative`
    * 자연스럽게 배치
    * 상대적인 위치를 이용
  * `absolute`
    * 원하는 요소에 위치
    * 부모 요소를 relative로 지정해 놔야 가능
  * `fixed`
    * 브라우저 창 기준
    * 창 스크롤 하더라도 같은 위치에 고정
* `visibility: visible`
* `z-index: 1`
    * 요소 쌓는 순서 정하기
### 다단으로 편집하기
* `column-width: <크기>`
  * 단의 너비를 고정해 놓고 화면 분할
* `column-count: <숫자>`
  * 단의 개수를 먼저 저애
* `column-rule: 2px dotted #ccc`
  * 단 사이의 줄
* `break-before: column`
  * 특정 요소 앞이나 뒤
  * 주로 인쇄 목적
* `column-span: 1`
  * 여러 단을 하나로 합치기

|속성 값|설명|
|:---:|:---:|
|1| 단을 하나만 합치는 것으로 합치지 않는 것과 같습니다. 기본 값입니다.|
|all| 전체 단을 하나로 합쳐 표현합니다.|


## 표 스타일
* `caption-side: top`
  * 설명글
  * 기본값: top
* `border: 1px solid black`
  * 표의 바깥 테두리와 셀 테두리를 모두 지정해야 함
* `border-collapse: separate`
  * 표 테두리와 셀 테두리를 합칠 것인지 결정

|속성 값|설명|
|:---:|:---:|
|collapse| 테두리를 하나로 합쳐 표시합니다.|
|separate| 테두리를 따로 표시합니다. 기본 값입니다.|

* `border-spacing: 20px 10px`
  * 표 테두리와 셀 테두리 사이의 거리를 지정
  * 값이 1개
    * 수평 & 수직 거리 같음
  * 값이 2개
    *  수평, 수직    
* `empty-cell: show`
  * 내용이 없는 빈 셀들의 표시 여부 지정
* `width: 300px` `height: 100px` `pedding: 10px`
* `table-layout: auto`
  * 셀 안의 내용 양에 따라 셀 너비를 변하게 할지, 고정시킬지 결정

|속성 값|설명|
|:---:|:---:|
|fixed| 셀 너비를 고정합니다. 즉, 셀 내용에 따라 셀의 너비가 달라지지 않습니다. |
|auto| 셀 내용에 따라 셀의 너비가 달라집니다. 기본 값입니다.|

* `text-align: left`
  * 셀 안에서의 수평 정렬 방법
* `vertical-align: middle`
  * 셀 안에서의 수직 정렬 방법

|속성 값|설명|
|:---:|:---:|
|top| 위쪽 패딩 가장자리에 내용의 윗부분을 맞춥니다.|
|bottom| 아래쪽 패딩 가장자리에 내용의 아랫부분을 맞춥니다.|
|middle| 패딩의 중앙에 내용의 중앙을 맞춥니다.|

## CSS3 선택자
### 연결 선택자
* 하위 선택자
  * `<상위요소 하위요소{color: blue;}>`
  * 부모 요소에 포함된 모든 하위 요소에 스타일이 적용
* 자식 선택자
  * `<부모요소 > 자식요소{color: blue;}>`
  * 자식 요소에만 스타일이 적용
  * 손자 요소에는 스타일 적용 안됨
* 인접 형제 선택자
  * `<요소1 + 요소2 {text-decoration: underline}>`
  * 첫번쨰 형제 요소에만 스타일이 적용
* 형제 선택자
  * `<요소1 ~ 요소2 {text-decoration: underline}>`
  * 모든 형제 요소에 스타일이 적용
* 속성 선택자
  * `a[속성]{background: yellow;}`
  * `a[속성=값]{background: yellow;}`
    * 지정한 속성(값)을 가진 요소를 찾아 스타일 적용
  * `a[속성~=값]{background: yellow;}`
    * 여러 속성 값 중에 해당 값이 포함되어 있는 요소를 찾아 스타일 적용
    * `class="button"` `class="flat button"`
  * `a[속성|=값]{background: yellow;}`
    * 특정 값이 포함된 속성을 가진 요소를 찾아 스타일 적용
    * 하이픈 포함 단어별
  * `a[속성^=값]{background: yellow;}`
    * 특정 값으로 시작하는 속성을 가진 요소를 찾아 스타일 적용
  * `a[속성$=값]{background: yellow;}`  
    * 특정 값으로 끝나는 속성을 가진 요소를 찾아 스타일 적용
  * `a[속성*=값]{background: yellow;}`
    * 값의 일부가 일치하는 속성을 가진 요소를 찾아 스타일 적용
### 가상 클래스
* 사용자 동작에 반응하는 가상 클래스
  * `:link`
    * 방문하지 않은 링크에 스타일 적용
  * `:visited`
    * 방문한 링크에 스타일 적용
  * `:hover`
    * 웹 요소에 마우스 커서를 올려놓을 때의 스타일 적용
  * `:active`
    * 웹 요소를 클릭했을 떄의 스타일 적용
  * `:focus`
    * 웹 요소에 초점이 맞추어졌을때의 스타일 적용
  * 나열된 순서대로 적용해야함
* UI 요소 상태에 따른 가상 클래스
  * `:enabled`
    `:disabled`
    * 요소를 사용할 수 있을 떄와 없을 떄의 스타일 지정
  * `:checked`
    * 라디오 박스나 체크 박스에서 항목을 선택했을 떄의 스타일 지정
* 구조 가상 클래스
  * `:nth-child(n)`
    * 앞에서부터 n번째 자식 요소에 스타일 적용
  * `:nth-last-child(n)`
    * 뒤에서부터 n번쨰 자식 요소에 스타일 적용
  * n 대신에 even, 2n+1, 2n+0 등 가능
  * `nth-of-type(n)`
    * 특정 태그 위치에 앞에서부터 스타일 적용
  * `nth-last-of-child(n)`  
    * 특정 태그 위치에 뒤에서부터 스타일 적용
  * `:first-child`
    * 첫번째 자식요소에 스타일 적용
  * `:last-child`
    * 마지막 자식요소에 스타일 적용
  * `:first-of-type`
    * 형제 요소들 중 첫번째 요소에 스타일 적용
  * `:last-of-type`  
    * 형제 요소들 중 마지막 요소에 스타일 적용
  * `:only-child`
    * 부모 요소 안에 자식 요소가 유일하게 하나일 떄 스타일 적용
  * `:only-of-type`
    * 자신이 유일한 요소일 떄 스타일 적용
  * `::first-line`
    * 특정 요소의 첫번째 줄에 스타일 적용
  * `::first-letter`
    * 특정 요소의 첫번쨰 글자에 스타일 적용
  * `::before`
    * `content:"내용";`
    * `content:url();`
    * 특정 요소의 앞에 지정한 내용을 추가
  * `::after`
    * 특정 요소의 뒤에 지정한 내용을 추가
  * **실제 브라우져 상에는 표현되지만 자바스크립트로 수정 불가**
