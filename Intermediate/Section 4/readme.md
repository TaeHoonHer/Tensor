## NN(Neural Network)
- NN에서 중요한 또다른 문제 : 회귀(Regression)
- NN의 경우 activation function을 삭제하면 바로 회귀 문제를 풀 수 있다

![image](https://user-images.githubusercontent.com/107015573/215405019-5b989fd6-1b44-4d70-80f8-56ced19853b6.png)

- input값과 가중치를 곱해서 더해진 summation의 범위는 –무한 ~ 무한이다. 이러한 연속값을 확률적으로 mapping하기 위해 사용하는 것이 앞에서 사용한 Softmax같은 Activation function이다.

확률값이 필요한 이유는 분류문제를 풀기 위해서, 그럼 회귀 문제를 풀 때는 확률 필요?
- 회귀 문제를 풀 때는 연속값을 그대로 놔둬서 연속값을 맞추라고하면된다.                           
- Linear Function을 Activation Function으로 썻다고 한다
- Linear Function = (y = x) 즉 들어온 값을 그대로 뱉었다

## Loss Function
- input으로 들어가서 hidden layer를 거치고 나온 Output값이 얼마나 잘 나왔나를 평가할 수 있는 항목

분류 : Cross-Entrophy
회귀 : MSE(Mean Squared Error)

![image](https://user-images.githubusercontent.com/107015573/215405286-8593c75f-e45b-4ef5-92b8-eef779468eb9.png)
