![image](https://github.com/uthem150/Card_Post_Web/assets/142042011/1c0c658e-1efc-4a6d-843e-3f070aac74e3)

<접속>
https://uthem150.github.io/Card_Post_Web/

게임 속에서 포켓몬 카드를 수집하는것 처럼,  
각 카드가 마우스의 움직임에 따라, 동적으로 변하는 카드 컬렉팅 웹  

----
A.  
카드 이미지 넣을 container 생성 후,  
카드 이미지를 넣음

B.  
container에 mousemove라는 이벤트 리스너를 추가해서  
마우스의 좌표를 받아오고(offsetX, offsetY)  
이에 따라서 container의 transform style속성을 변경해서  
<마우스 좌표에 따라서 이미지가 회전> 기능 구현  
  
x좌표가 200px에 위치하면, rotateY를 -20degree  
x좌표가 0px에 위치하면, rotateY를 20degree  
이 되도록, 1차 방정식 생성 (rotateY = -1/5 * x + 20) (rotateX = 4/30 * y - 20)
+ 3D요소를 시각화하기 위해, perspective 속성 추가함(원근 효과)  
  
C.  
무지개 필름 느낌을 주기 위해서
overlay라는 클래스를 만들고
마우스가 움직임에 따라서 함께 필름도 움직이는 모습을 표현하기 위해  
background-position속성을 조정해줌

  

