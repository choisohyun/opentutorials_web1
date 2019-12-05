# 생활코딩 공부
- 생활코딩 WEBn 강좌를 [WEB1 - HTML & Internet](https://opentutorials.org/course/3084)부터 차례대로 수강하여 적용시킨 웹페이지입니다.
- 코드는 생활코딩에서 제공하는 예제 코드와 동일합니다.
- Markdown 활용하여 공부 내용을 날짜별로 정리합니다.
- 웹페이지 방문하기 - [클릭](https://choisohyun.github.io/opentutorials_web1/)
## 수정 내역
- 2019.11.27 
  - [WEB1 - HTML & Internet](https://opentutorials.org/course/3084) 완강 후 적용
  - 간단한 초기 웹페이지
  - `index.html`과 3개의 부속 페이지로 구성
- 2019.12.03 
  - [WEB2 - CSS](https://opentutorials.org/course/3086)의 [CSS 코드의 재사용](https://opentutorials.org/course/3086/18327)까지 적용
  - 초기 웹페이지에 `style.css` 가 추가됨
- 2019.12.05
  - [WEB2 - JavaScript](https://opentutorials.org/course/3085/) [객체 활용](https://opentutorials.org/course/3085/18885)까지 적용
  - 기존 상태에서 `colors.js`가 추가됨
  - 알게 된 점 - 아래와 같이 함수가 객체의 한 요소로 들어가 `Links.setColor('white');`의 형태로 호출될 수 있다는 것.
    ```
    var Links = {
      setColor:function(color){
        var alist = document.querySelectorAll('a');
        var i = 0;
        while(i < alist.length){
          alist[i].style.color = color;
          i = i + 1;
        }
      }
    } 
    ```
- 2019.12.05
  - [WEB2 - JavaScript](https://opentutorials.org/course/3085/) 완강 후 적용
  - 기존의 js 파일에서 jQuery 문법을 적용시킴
    ```
    var Links = {
      setColor:function(color){
        $('a').css('color', color);
      }
    }
    ```
