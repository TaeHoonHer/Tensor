### What is Neural Network?
- 인간 뇌의 기능을 묘사한 것
  - data : 자극이 입력기관을 통해 뇌로 입력
  - activation : 자극이 들어오면 뉴런이 활성화
  - weight : 같이 활성화되는 뉴련들은 강하게 연결된다


### Linear Separability : 선형 분리 가능성(binary classification)
- What can we do with one single line?
  - 우리는 선 하나로 무엇을 할 수 있을까?

<img src= "https://user-images.githubusercontent.com/107015573/215021129-93f024c2-afcb-4080-accd-180d8e71f5d3.png" width="200" height="220">
공간을 분할, class를 분류할 수 있다

- 빨간 부분 : y = f(x) > 0
- 파란 부분 : y = f(x) < 0

이를 구분하는 수식 
- $g(x_1, x_2) = w_1 x_1 + w_2 x_2 + w_0 = 0$
-- x1, x2 값에 w1, w2 가중치를 곱한 후 w0(절편 == 인터셉트 == 바이어스)를 더한다

위 수식을 그림으로 설명하면
![image](https://user-images.githubusercontent.com/107015573/215022202-012124ba-fbe2-4e8c-bcd5-8ed3ceefd86a.png)
- x1, x2로 받아들이는 input값에 w1, w2 가중치를 곱하고, 해당 값에 w0 절편을 더해 값이 0보다 크면 위, 작으면 아래로 class를 구분한다

![image](https://user-images.githubusercontent.com/107015573/215022328-138145d4-b94c-4889-9ff3-25132c24f706.png)
그림 설명
>- 입력 I개
>- 가중치 I개
>- 절편 1개
>>- 연산이 된 값들이 더해져 Summation(가중합) 진행
>>- 가중합 상태에서 어느 영역에 속하는지 판단
>>    - How?
>>    - Using Activation Function(활성함수) : 공간을 분할한다
   
활성함수(Activation Function)
- 0보다 크면 1, 작으면 0 또는 -1이라는 값을 내보낸다
![image](https://user-images.githubusercontent.com/107015573/215389023-48c363b6-3324-4cc0-815d-707b16d66fd6.png)

- Threshold(Step function) : 미분이 불가능
- Logistic : Step Function에서 미분이 가능하도록 만들어짐
  - 단점 : 0과 1 사이에서 해결이 안되는 것들이 있다
- Tanh : 범위를 음수의 영역까지 늘린 것
![image](https://user-images.githubusercontent.com/107015573/215389292-f1ecf285-67f4-4ab3-b0bc-9e9ab14f41d1.png)
x 1,2,3번이 있다
각 위치에 해당하는 값에 절편(-1.5)를 넣어 계산하면 위에 표와 같이 각 활성함수마다 값이 다르게 나온다
