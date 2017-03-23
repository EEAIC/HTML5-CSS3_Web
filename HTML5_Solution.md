HTML5
===
Basic
----
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

* <code>`<!doctype html>` or `<!doctype html>`</code>
  * Html 문서이고 버전임을 명시
* <code>`<html>`</code>
  * 실제 문서 정보와 내용이 시작되고 끝나는 것을 표시하는 태그
  * <code> `<html lang="ko">`</code>
    * 사용할 언어 지정
* <code>`<head>`</code>
  * 웹 브라우저 화면상에는 보이지 않음
  * <code>`<title>`</code>
    * 제목 표시줄에 표시되는 내용
  * <code>`<meta>`</code>
    * 문자 인코딩 방법 및 요약 정보
  * <code>`<meta charset="utf-8">`</code>
* <code>`<body>`</code>
  * 실제 표시될 내용 부분

## 텍스트 태그

* <code>`<hn>`</code>
  * 제목을 표시할 때 사용하는 태그
  * n이 작을수록 글잨 크기가 큼
* <code>`<p>`</code>
    * 텍스트 단락
* <code>`<br>`</code>
    * 줄 바꾸기
    * 닫는 태그 없음
* <code>`<blockquote>`</code>
    * 인용문 넣기
    * 들여 쓰여짐
* <code>`<hr>`</code>
    * 수평줄 생김
    * 주제가 바뀔 때 전환 효과
    * 닫는 태그 없음
* <code>`<pre>`</code>
    * 소스에 표시한 공백 그대로 표시
* <code>`<strong>, <b>`</code>
    * <code>`<strong>`</code>
      * 중요한 내용
    * <code>`<b>`</code>
      * 단순히 굵게
* <code>`<em>, <i>`</code>
   * <code>`<em>`</code>
      * 특정 부분 강조
   * <code>`<i>`</code>
      * 단순히 이탤릭체
* <code>`<q>`</code>
    * 인용 내용 앞뒤에 (" ") 추가됨
    * 줄바꿈 없이 한줄에 인용 표시
* <code>`<mark>`</code>
    * 형광펜 효과
* <code>`<span>, <div>`</code>
    * CSS를 부분적으로 적용
    * <code>`<span>`</code>
      * 줄 안에서 묶기
    * <code>`<div>`</code>
      * 블럭으로 묶기
* <code>`<ruby><rt>`</code>
    * <code>`<rt>`</code>
      * 주석 표시      
* <code>`<ui>, <li>`</code>
    * 순서 없는 목록
* <code>`<oi>, <li>`</code>
    * 순서 있는 목록
    * <code>`type="a"`</code>
    * <code>`start="1"`</code>
    * <code>`reserved`</code>
* <code>`<dl>,<dt>,<dd>`</code>
    * 설명 목록
    * <code>`<dt>`</code>
      * 제목
    * <code>`<dd>`</code>
      * 내용
* <code>`<table>, <tr>, <td>, <th>`</code>
    * 표 만들기
    * <code>`<caption>`</code>
      * 표 이름
      * 이름은 하나만 가능
      * 중앙에 정렬
    * <code>`<tr>`</code>
      * 행
    * <code>`<td>`</code>
      * 셀
    * <code>`<th>`</code>
      * 제목이 있는 셀
    * <code>`border="1"`</code>
      * 표 테두리
* <code>`<figure>`</code>
    * <code>`<figcaption>`</code>
      * 대상에 이름 설정
      * 중앙에 정렬되지 않음
* <code>`colspan="3", rowspan="3"`</code>
    * <code>`colspan="3"`</code>
      * 행 합치기
    * <code>`rowspan="3"`</code>
      * 열 합치기
* <code>`<thead>, <tbody>, <tfoot>`</code>
    * 표 구조 정의
    * <code>`<thead>`</code>
      * 표 안에서의 제목 정의
    * <code>`<tbody>`</code>
      * 표 안에서의 내용 정의
    * <code>`<tfoot>`</code>  
      * 표 안에서의 요약 정의
    *  <code>`<tbody>`</code> 와 <code>`<tfoot>`</code> 은 순서 상관 없음
* <code>`<col>, <colgroup>`</code>
    * <code>`<tr>, <td>`</code> 전에 사용
    * 묶는 열의 개수 만큼 <code>`<col>`</code> 사용
    * <code>`<col>`</code>
      * 한 열의 모든 셀에 같은 스타일 적용
      * <code>`span="2"`</code>
        * 여러 열 묶기
      * 닫는 태그 없음

## 이미지 태그

* <code>`<img src="경로"`></code>
  * 이미지 삽입
  * <code>`alt="홈으로 가기"`</code>
    * 이미지를 설명하는 대체 텍스트
    * 이미지 표시 불가시 표시
    * 화면 낭독기가 읽음
  * <code>`width="숫자", height="숫자"`</code>
    * 이미지 크기 조정
    * 이미지 용량은 그대로

## 하이퍼링크

* 외부 사이트나 외부 페이지로 연결
* <code>`<a href="링크할 주소"> 텍스트나 이미지태그`</code>
  * <code>`target="_blank"`</code>
    * 링크 내용이 새 창이나 새 탭에서 열림
  * 앵커
    * <code>`<태그 id="앵커"> 텍스트 또는 이미지태그`</code>
      <code>`<a href="#앵커"> 텍스트 또는 이미지태그`</code>
    * 한 페이지 안에서 이동하기
* 이미지맵
  * 한 이미지 안에 여러 링크 만들기
  * <code>`<img src="경로 또는 주소" usemap="#맵이름">`</code>
  * <code>`<map name="맵이름">`</code>
  * <code>`<area shape="rect" coords="10,10,160,200 href="링크할 주소">`</code>
    * <code>`shape="rect"`</code>
    * <code>`coords="10,10,160,200"`</code>

  

## 폼

* 웹 사이트로 정보를 보낼 수 있는 요소들
* 정보를 저장 및 검색 또는 수정
* 사용자 정보를 처리하는 것은 ASP나 PHP 같은 서버 프로그래밍
* <code>`<form method="post">`</code>
  * <code>`method="get"`</code>
    * 입력한 부분이 주소표시줄에 나타남
    * 4096byte의 길이 제한
  * <code>`method="post"`</code>
    * 입력한 내용이 드러나지 않음
    * 길이 제한 없음
  * <code>`action="search.php"`</code>
    * 폼 안의 내용을 처리하는 서버 상의 프로그램
* <code>`<label>`</code>
  * 입력 필드 옆에 표시 되는 부분
  * 폼 전체를 묶어서 사용하거나 폼과 연결하여 사용 가능
    * <code>`<label for="user-id">`</code>
* <code>`<fieldset>`</code>
* 폼 요소를 그룹으로 묶는 태그
  * <code>`<legend>`</code>
  * 그룹으로 묶는 구역에 제목을 붙이는 태그
* <code>`<input type="유형">`</code>
  * 사용자가 내용을 입력하는 부분
  * <code>`type="hidden"`</code>
    * 화면 상에는 보이지 않음
    * 서버로 함께 전송되는 요소
  * <code>`type="password"`</code>
    * 비밀번호 입력란
  * <code>`type="text"`</code>
    * 한 줄짜리 텍스트 입력 필드
    * 주로 아이디나 이름, 주소 등 텍스트 입력
  * <code>`name="이름"`</code>
    * 텍스트 필드를 구별
  * <code>`size="5"`</code>  
    * 텍스트 필드의 길이를 지정
  * <code>`value="내용"`</code>  
    * 텍스트 필드 부분에 표시될 내용
    * 패스워드 필드에는 없음
  * <code>`maxlength="50"`</code>
    * 입력할 수 있는 최대 문자 개수
  * <code>`type="search"`</code>
    * 검색 필드
    * 검색어 삭제 쉬움
    * 주로 모바일에서 지원
  * <code>`type="email"`</code>
    * 메일 주소 형식 자동 체크
    * 메일 주소 입력 필드
  * <code>`type="url"`</code>
    * 사이트 형식 자동 체크
  * <code>`type="tel"`</code>
    * 전화번호 입력
  * <code>`type="radio"`</code>
    * 여러 항목중 하나만 선택
    * <code>`name="이름"`</code>
      * 모두 같아야 함
    * <code>`value="내용"`</code>
      * 서버에 전달될 값
  * <code>`type="checkbox"`</code>
    * 여러 항목 중 둘 이상 선택
    * <code>`name="이름"`</code>
      * 모두 달라야 함
    * <code>`value="내용"`</code>
      * 서버에 전달될 값
  * <code>`type="submit"`</code>
    * 폼 전송
    * 입력 내용을 서버로 전송
    * 사용자 입력 내용 전부 삭제
  * <code>`type="reset"`</code>
    * 사용자 입력 내용 전부 삭제
  * <code>`type="image"`</code>
    * submit 버튼 대신 이미지 삽입
  * <code>`autofocus`</code>
    * 원하는 폼 요소에 마우스 커서 표시
  * <code>`placeholder="하이픈없이 입력"`</code>
    * 입력란에 표시하는 힌트로, 필드를 클릭하면 사라짐
  * <code>`readonly`</code>
    * 폼 형식
    * 입력하지 못함
  * <code>`required`</code>
    * 필수 필드 체크
  * <code>`min="10", max="100"`</code>
    * 최소값, 최대값
    * 태그 유형이 date, datetime, datetime-local, month, week, time, number, range일 경우에만 사용
  * <code>`step="2"`</code>
    * 허용된 범위 내의 숫자의 일정한 간격
    * 태그 유형이 date, datetime, datetime-local, month, week, time, number, range일 경우에만 사용
  * <code>`<select>`</code>
    * 여러 옵션 중 하나 이상을 선택 가능
    * <code>`<option>`</code>
      * 드롭다운 목록
    * <code>`<optgroup>`</code>
      * 여러 항목을 그룹으로 묶음
  * <code>`<datalist id="choices">`</code>
    * **input** 의 **list** 속성에 **id** 를 입력하여 값이 자동으로 입력되게 할 수 있음
    * 사용자가 직접 텍스트 필드 입력 가능
  * <code>`<textarea>`</code>
    * 여러 줄의 텍스트 입력
    * <code>`cols="100", rows="100"`</code>
      * 가로 너비 지정 가능
  * <code>`<button>`</code>
    * 다양한 형태의 버튼 삽입
* <code>`<output>`</code>   
  * 계산 결과를 브라우저에 표시
  * 웹 브라우저가 계산의 결과값인 것을 정확히 인지
* <code>`<progress>`</code>
  * 작업 진행 상태를 브라우저에 표시
  * <code>`max="60"`</code>
  * <code>`value="50"`</code>
    * 작업의 진행의 현재 상태
* <code>`<meter>`</code>
  * 전체 크기 중 얼마나 차지하는지를 표시
  * <code>`low="100", high="1024"`</code>
  * <code>`optimum="0.8"`</code>
    * **optimum** 값이 **high** 값보다 크면 **value** 값이 클수록 좋고 **low** 보다 작으면 **value** 값이 작을수록 좋음










#### 웹 문서 업로드

* FTP 프로그램
  * 각종 파일을 서버로 업로드하거나 다운로드
