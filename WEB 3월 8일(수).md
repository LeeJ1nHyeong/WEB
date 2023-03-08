# 3/8(수)

## CSS

#### CSS 원칙 1

* 모든 요소는 네모(박스모델)이고 위에서부터 아래로, 왼쪽에서 오른쪽으로 쌓인다.



### Box model

* 모든 HTML 요소는 box 형태로 되어있음

* 하나의 박스는 네 부분(영역)으로 이루어짐

  * content : 글이나 이미지 등 요소의 실제 내용
  * padding : 테두리 안쪽의 내부 여백, 요소에 적용된 배경색, 이미지는 padding까지 적용
  * border : 테두리 영역
  * margin : 테두리 바깥의 외부 여백, 배경색 지정 불가

* Box model 구성

  ```css
  /* margin */
  .margin {
    margin-top: 10px;
    margin-right: 20px;
    margin-bottom: 30px;
    margin-left: 40px;
  }
  
  .margin-1 {
    margin: 10px; /* 상하좌우 다 10px */
  }
  
  .margin-2 {
    margin: 10px 20px;  /* 상하 10 좌우 20 */
  }
  
  .margin-3 {
    margin: 10px 20px 30px;  /* 상 10 좌우 20 하 30 */
  }
  
  .margin-4 {
    margin: 10px 20px 30px 40px;  /* 상부터 시계방향으로 적용 (상 10 우 20 하 30 좌 40) */
  }
  
  /* padding */
  .margin-padding {
    margin: 10px;
    padding: 30px;
  }
  
  /* border */
  .border {
    border-width: 2px;
    border-style: dashed;
    border-color: black;
  }
  ```

* box-sizing
  * 기본적으로 모든 요소의 box-sizing은 content-box
    * Padding을 제외한 순수 contents 영역만을 box로 지정
  * 다만, 우리가 일반적으로 영역을 볼 때는 border까지의 너비를 100px 보는 것을 원함
    * 그 경우 box-sizing을 border-box로 설정



### CSS Display

#### CSS 원칙 2

* display에 따라 크기와 배치가 달라진다.





* 가운데 정렬 방법
  * margin : 0px auto → 블록 요소를 가운데 정렬할 때
  * '부모 요소'에 text-align : center → 인라인 요소를 가운데 정렬할 때