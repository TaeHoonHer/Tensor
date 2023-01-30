### Perceptron(퍼셉트론)
- 입력값에 가중치를 곱해 절편을 더하고 활성화 함수로 구분하는 것

![image](https://user-images.githubusercontent.com/107015573/215389556-07988d90-ed40-4fd1-bd67-482395951b1a.png)

Single Perceptron은 Linear Separability(직선구분)을 활용해 구분을 하는데, 직선으로 풀리지 않는 문제들이 있다
![image](https://user-images.githubusercontent.com/107015573/215390304-fed32322-de68-4a8c-ad8e-fa46c8c93c1a.png)
위에 사진처럼 대표적으로 Xor Problem이 있다
Xor에서는 직선을 어떤 방식으로 그어도 문제가 하나는 무조건 발생한다
이를 NonLinear Problem이라고 부른다

해결방법
- Perceptron을 여러개 중첩해서 사용한다면 어떨까? : Multi-layer Perceptron

Multi-layer Perceptron(MLP)
- Single layer Perceptron으로 해결이 되지 않는 문제들을 여러개의 perceptron을 중첩시켜서 해결하는 방식
![image](https://user-images.githubusercontent.com/107015573/215391098-33ff9797-94b1-44df-89a0-2185165fa488.png)
![image](https://user-images.githubusercontent.com/107015573/215391128-04bbf901-d6e9-4a5a-a026-54bcee4eb648.png)
![image](https://user-images.githubusercontent.com/107015573/215391152-d3d228a3-d6ef-4f5a-b3dd-8ac71f558685.png)
Single Layer Perceptron으로는 어려운 문제를 해결할 수 없지만, MLP로는 가능하다

- MLP에서 문제점
  - MLP에서 가중치를 구하는 방법은 무엇일까?
