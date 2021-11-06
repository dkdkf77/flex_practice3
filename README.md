# flex_practice3

패스트 캠퍼스 front-end 강의 중 flex 속성에 대한 공부

<hr/>

### item에 줄 수 있는 속성 들

- flex-grow : 주 축의 너비가 즉 수평의 너비가 1:1:1 비율로 늘어난다. 기본 값 : 0

  ![스크린샷 2021-10-30 오후 3 52 30](https://user-images.githubusercontent.com/88579497/139524586-369203bd-f921-4cfe-9cc3-df594cfc8952.png)

- 3번째 item에 flex-grow: 2 를 줬을 시

  ![스크린샷 2021-10-30 오후 3 55 24](https://user-images.githubusercontent.com/88579497/139524587-ef8d500a-3a03-479b-99c9-d435c9a3b336.png)

- 1:1:1 비율이 아니게 된다. 그럴때는 flex-basis: 0;을 주게 되면 1:1:2 의 비율을 줄 수 있다.

  ![스크린샷 2021-10-30 오후 3 56 45](https://user-images.githubusercontent.com/88579497/139524591-b5ac3de2-cccf-41a3-b234-54556e22b23c.png)


<hr/>

### order : flex item의 순서

기본 값 0,
숫자 설정 - 숫자가 작을 수록 먼저

- 0보다 작은 수를 적어도 된다 예를 들어 -1 등
- -1 > 3 > 10 숫자가 기본 값 보다 작은 순서 대로 정렬 된다.
  
  ![스크린샷 2021-10-30 오후 4 02 56](https://user-images.githubusercontent.com/88579497/139524601-99ed9ad2-ba1a-46c2-ad80-3e2f3cbc72e3.png)


장점 : html 구조를 바꾸지 않고도 화면에 출력되는 순서를 바꿀 수 있다는 점

<hr/>

### flex-shrink : flex item의 감소 너비 비율

기본 값 1 - flex container 너비에 따라 감소 비율 적용
숫자 설정 - 감소 비율

- flex 를 사용하여 수평정렬을 했을때 너비가 부족하면 네모가 찌르러 질껀데 요소들이 찌그러지지 않게 하고 싶으면 각각의 item에다 flex-shrink 값을 기본 값 1이 아닌 0으로 주면 찌그러지지 않게 된다.

<hr/>

### flex-basis : flex item의 공간 배분 전 기본 너비 (출처 - 패스트 캠퍼스 강의 내용 중)

<img width="790" alt="스크린샷 2021-10-30 오후 4 28 08" src="https://user-images.githubusercontent.com/88579497/139524634-3ec1ed31-adaf-4c99-b3f6-56cdb1014946.png">


auto - 요소 Content 너비 (내용의 너비)
단위 - px,em, rem emd 등 단위로 지정

- 0으로 사용 시

<img width="612" alt="스크린샷 2021-10-30 오후 4 28 48" src="https://user-images.githubusercontent.com/88579497/139524655-c44915fb-d7f1-4350-a638-ec29c5d15559.png">

- px 로 사용 시

<img width="786" alt="스크린샷 2021-10-30 오후 4 29 40" src="https://user-images.githubusercontent.com/88579497/139524661-5540aca5-8e88-4596-953d-8d864f5532c5.png">


