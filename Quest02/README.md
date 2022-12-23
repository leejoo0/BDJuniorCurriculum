# Quest 02. CSS의 기초와 응용

## Introduction

* CSS는 Cascading StyleSheet의 약자입니다. 웹브라우저에 표시되는 HTML 문서의 스타일을 지정하는 (거의) 유일하지만 다루기 쉽지 않은 언어입니다. 이번 퀘스트를 통해 CSS의 기초적인 레이아웃 작성법을 알아볼 예정입니다.

## Topics

* CSS의 기초 문법과 적용 방법
  * Inline, `<style>`, `<link rel="stylesheet" href="...">`
* CSS 규칙의 우선순위
* 박스 모델과 레이아웃 요소
  * 박스 모델: `width`, `height`, `margin`, `padding`, `border`, `box-sizing`
  * `position`, `left`, `top`, `display`
  * CSS Flexbox와 Grid
* CSS 표준의 역사
* 브라우저별 Developer tools

## Resources

* [MDN - CSS](https://developer.mozilla.org/ko/docs/Web/CSS)
* [Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)
* [A complete guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [그리드 레이아웃과 다른 레이아웃 방법과의 관계](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Grid_Layout/%EA%B7%B8%EB%A6%AC%EB%93%9C_%EB%A0%88%EC%9D%B4%EC%95%84%EC%9B%83%EA%B3%BC_%EB%8B%A4%EB%A5%B8_%EB%A0%88%EC%9D%B4%EC%95%84%EC%9B%83_%EB%B0%A9%EB%B2%95%EA%B3%BC%EC%9D%98_%EA%B4%80%EA%B3%84)

## Checklist

* CSS를 HTML에 적용하는 세 가지 방법은 무엇일까요?
  * ```
    Inline Style Sheet : HTML 태그에 style 속성에 코드를 넣는 방법
    Internal Style Sheet : <style> 코드 안에 CSS 넣는 방법
    Linking Style Sheet : CSS 파일을 만들고 HTML 문서와 연결하는 방법
  * 세 가지 방법 각각의 장단점은 무엇일까요?
  * ```
    Inline Style Sheet : 장점 - 개별 설정이 가능하다. 단점 - 꾸미는것에 한계가 있고 재사용이 불가능하다.
    Internal Style Sheet : 문서 안에 여러 요소를 한번에 수정이 가능하지만 또다른 HTML 문서에는 적용 할 수 없다.
    Linking Style Sheet : 여러 HTML 문서에 사용가능 하다. 
    
* CSS 규칙의 우선순위는 어떻게 결정될까요?
  * ```
    뒤에 나오는 css 우선순위가 높다.
    !important > inline style attribute > id > class, 다른 attribute, 수도클래스(:first-child같은 것) > tag element, 수도엘레먼트(::before같은 것) 순으로 우선순위가 높다.
    우선순위가 같다면 개수가 많은 css가 우선순위가 높다.
    
* CSS의 박스모델은 무엇일까요? 박스가 화면에서 차지하는 크기는 어떻게 결정될까요?
  * ```
    모든 HTML 요소는 박스 모양으로 구성된다. Padding, border, margin , content 로 구분한다
    박스는 설정된 치수와 내용 등 콘텐츠 크기를 기반으로 결정 된다.순수하게 content 영역의 너비만을 포함한다.
    실제 엘리먼트가 화면에서 차지하는 너비를 생각할 때는 padding과 border의 두께까지 고려해야한다.
* `float` 속성은 왜 좋지 않을까요?
  * ```
    부모요소가 자식 요소의 크기를 반영하지 못한다, 부모요소의 높이가 초기화되어 사라진다.
* Flexbox(Flexible box)와 CSS Grid의 차이와 장단점은 무엇일까요?
  * ```
    Flexbox : 수평, 수직 영역 중 하나의 방향으로만 레이아웃을 나눌 수 있음
    Grid : 수평 수직을 동시에 영역을 나눌 수 있음
* CSS의 비슷한 요소들을 어떤 식으로 정리할 수 있을까요?
  * ``` 
    선택자를 사용해서 정리.

## Quest

* Quest 01에서 만들었던 HTML을 바탕으로, [이 그림](screen.png)의 레이아웃과 CSS를 최대한 비슷하게 흉내내 보세요. 꼭 완벽히 정확할 필요는 없으나 align 등의 속성은 일치해야 합니다.
* **주의사항: 되도록이면 원래 페이지의 CSS를 참고하지 말고 아무것도 없는 백지에서 시작해 보도록 노력해 보세요!**

## Advanced

* 왜 CSS는 어려울까요?
* CSS의 어려움을 극복하기 위해 어떤 방법들이 제시되고 나왔을까요?
* CSS가 브라우저에 의해 해석되고 적용되기까지 내부적으로 어떤 과정을 거칠까요?
* 웹 폰트의 경우에는 브라우저 엔진 별로 어떤 과정을 통해 렌더링 될까요?
