# Quest 01. HTML과 웹의 기초

## Introduction

* HTML은 HyperText Markup Language의 약자로, 웹 브라우저에 내용을 표시하기 위한 가장 기본적인 언어입니다. 이번 퀘스트를 통해 HTML에 관한 기초적인 사항들을 알아볼 예정입니다.

## Topics

* HTML의 역사
  * HTML 4.01, XHTML 1.0, XHTML 1.1
  * XHTML 2.0과 HTML5의 대립
  * HTML5와 현재
* 브라우저의 역사
  * Mosaic와 Netscape
  * Internet Explorer의 독점시대
  * Firefox와 Chrome의 등장
  * iOS Safari와 모바일 환경의 브라우저
  * Edge와 Whale 등의 최근의 Chromium 계열 브라우저
* HTML 문서의 구조
  * `<html>`, `<head>`와 `<body>` 등의 HTML 문서의 기본 구조
  * 시맨틱 엘리먼트
  * 블록 엘리먼트와 인라인 엘리먼트의 차이

## Resources

* [MDN - HTML](https://developer.mozilla.org/ko/docs/Web/HTML)
* [HTML For Beginners](https://html.com/)
* [History of the web browser](https://en.wikipedia.org/wiki/History_of_the_web_browser)
* [History of HTML](https://en.wikipedia.org/wiki/HTML)
* [StatCounter](https://gs.statcounter.com/)

## Checklist

* HTML 표준의 역사는 어떻게 될까요? 
    - ``` 
      1980년, 유럽 입자 물리 연구소(CERN)의 계약자였었던 물리학자 팀 버너스리가 HTML의 원형인 인콰이어를 제안
      논문을 보기 위하여 만듬

    * HTML 표준을 지키는 것은 왜 중요할까요?
      ```
       소스의 통일화로 수정 및 운영관리가 용이
    * XHTML 2.0은 왜 세상에 나오지 못하게 되었을까요?
      ```
      XML(eXtensible Markup Language)은 버전과 버전사이의 하위 호환성을 지원하지 않아서 호환문제와 사용성 측면에서 단점이있었음.
    * HTML5 표준은 어떤 과정을 통해 정해질까요?
      ```
       World Wide Web Consortium (W3C) 에서 사용자불편 반영해서 발표
    * 브라우저의 역사는 어떻게 될까요?

        ``` 최초의 웹 브라우저는 1990년에 팀 버너스 리가 발명하였다. HTMl 문서 파일을 출력하는 응용소프트웨어이다.```

      * Internet Explorer가 브라우저 시장을 독점하면서 어떤 문제가 일어났고, 이 문제는 어떻게 해결되었을까요?
        ``` 
        * Internet Explorer 최적화되어 다른 웹브라우저로 들어가면 화면이 이상해지거나 깨지는 호환문제 발생.(호환성)
        Internet Explorer 는 표준을 지키지 않은 자신만의 표준을 만들어 버림 (비표준)
        기능 업데이트 되지 않고 기술이 발전하지 않음
        * 새로운 브라우저가 부상되어 독점 해소.

      * 현재 시점에 브라우저별 점유율은 어떻게 될까요? 이 브라우저별 점유율을 알아보는 것은 왜 중요할까요?
        ``` 
           2022 기준 크롬(Chrome)이 약 67% (66.93%)로 압도적으로 1위를 차지했고, 엣지(Edge)가 약 11% (10.63%), 사파리(Safari)가 약 9% (8.95%), 파이어폭스(Firefox)가 약 8% (7.8%), 오페라(Opera)가 약 3%(2.99%), ID(Internet Explorer)가 약 1% (0.75%)를 차지하였습니다.
      * 브라우저 엔진(렌더링 엔진)이란 무엇일까요? 어떤 브라우저들이 어떤 엔진을 쓸까요?
        ```
        요청된 컨텐츠들을 브라우저 화면에 표시한다 (html, img , XML)
        브라우저는 각기다른 렌더링 엔진을 사용한다.
        webkit이 보편적으로 사용된다.
      * 모바일 시대 이후, 최근에 출시된 브라우저들은 어떤 특징을 가지고 있을까요?
        ```
        반응형, 소형화,사용자 편의성 고려, 빠른속도
      * HTML 문서는 어떤 구조로 이루어져 있나요?
      * ```
         <html>, <head> , <body> 로 구성되어 있음. 
         ```
      * `<head>`에 자주 들어가는 엘리먼트들은 어떤 것이 있고, 어떤 역할을 할까요? 
        ```
        meta : 메타데이터
        title : 제목 달기 
        link : 이미지, 스타일시트 등 
      * 시맨틱 태그는 무엇일까요?
         ```  
        의미가 있는 태그. 이름만 봐도 어떤 태그인지 알 수 있음
        SEO (검색) , 웹접근성 , 유지보수성 활용에 좋다.
    
      * 시맨틱 엘리먼트를 사용하면 어떤 점이 좋을까요?
        ```
        검색 엔진은 의미론적 마크업 을 페이지의 검색 랭킹에 영향을 줄 수 있는 중요한 키워드로 간주
        시각 장애가 있는 사용자가 화면 판독기로 페이지를 탐색할 때 의미론적 마크업을 푯말로 사용할 수 있다.
        의미없고 클래스 이름이 붙여져있거나 그렇지 않은 끊임없는 div들을 탐색하는 것보다, 의미있는 코드 블록을 찾는 것이 훨씬 쉽다.
        의미있는 이름짓기(Semantic naming)는 적절한 사용자 정의 요소 / 구성 요소의 이름짓기(namimg)를 반영한다.
        
      * `<section>`과 `<div>`, `<header>`, `<footer>`, `<article>` 엘리먼트의 차이점은 무엇인가요?
        * ```
          section : 한페이지 안에 여러 내용을 보여주고 연관있는 내용을 묶어서 보여줄 때 사용 할 수 있음  
          footer : 부가적인 정보나 링크를 포함 할 수 있음
          header : 제목 웹사이트로고 검색폼 작성자 이름 등을 포함 할 수 있음
          article : 독립적인 정보를 나타낼 깨 사용 할 수 있음
          div : 구간 나누기 


          
        * 블록 레벨 엘리먼트와 인라인 엘리먼트는 어떤 차이가 있을까요?
          ```
          블록 엘리먼트 : 
          줄바꿈 되지 않고 그 자체로 한줄을 완전히 차지한다. 기본적으로 width 값이 100% 로 설정 된다.
          p, h1~h6, ul, ol, dl, table, div, noscript, blockquote, form, hr, table, fieldset, adress


          인라인 엘리먼트 : 
          줄을 바꾸지 않고 다른 요소와 함께 수평으로 한 행에 정렬하려는 속성 이다.
          samp, kbd, var, cite, abbr, acronym, a, img, object, br, script, map, q, sub, sup, span, bdo, input, select, textarea, label, button
          
          인라인 : 줄바꿈을 하지 않는다.
          블록 : 무조건 한 줄을 점유 다음 태그는 무조건 줄바꿈이 적용

## Quest

* [이 화면](screen.png)의 정보를 HTML 문서로 표현해 보세요. 다만 CSS를 전혀 사용하지 않고, 문서의 구조가 어떻게 되어 있는지를 파악하여 구현해 보세요.
  * [CSS Naked Day](https://css-naked-day.github.io/)는 매년 4월 9일에 CSS 없는 웹 페이지를 공개하여 내용과 마크업에 집중한 HTML 구조의 중요성을 강조하는 행사입니다.
* 폴더에 있는 `skeleton.html` 파일을 바탕으로 작업해 보시면 됩니다.
  * 정확하게 구현할 필요는 없습니다. 구조를 파악하는데 집중해봅시다.
  * 화면을 구성하는 큰 요소들을 어떻게 처리하면 좋을까요?
  * HTML 문서상에서 같은 층위에 비슷한 요소들이 반복될 때는 어떤 식으로 처리하는 것이 좋을까요?

## Advanced

* XML은 어떤 표준일까요? 어떤 식으로 발전해 왔을까요?
  ```
  웹을 위한 응용 프로그램 제작을 위해 개발된 공식 표준 언어
  웹 환경에서 문서를 저장하고 원하는 정보를 검색하는 등 다양한 목적으로 발전
* YML, Markdown 등 다른 마크업 언어들은 어떤 특징을 가지고 있고, 어떤 용도로 쓰일까요?
    ```
  Yaml은 Yaml Ain't Markup Language라는 뜻으로 'YAML은 마크업 언어가 아니다'라는 재귀적 말장난 같은 이름을 가지고 있다.
  데이터 중심
  Markdown은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다. 특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있다. 
  