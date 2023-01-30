### Hidden Layer & Node란?
- Hidden Layer
  - input 공간을 몇 개의 작은 서브공간으로 나눈다
  - Hidden Layer가 많다는 것은 더 많은 step에 걸쳐 서브공간을 공략
Hidden Layer가 많다 == 더 해결할 수 있는 문제들이 늘어난다 == 능력치가 올라간다

> Hidden Node
> - 서브공간에서의 decision rule을 의미
> - Hidden Node가 많으면 decision rule을 더 많이 조합한다는 의미
Hidden Layers and Nodes가 많다면 == Overfiting 발생

## FeedForward
![image](https://user-images.githubusercontent.com/107015573/215404150-2bc6c78d-6603-4bc7-9513-65c93353cc9f.png)

정보가 input으로 들어가서 Output으로 나오는, 한방향으로 흐른다
(정보는 한 방향(feedforward)으로만 흐른다)

![image](https://user-images.githubusercontent.com/107015573/215404187-174b0bb0-21f1-42c2-8d9a-75dbda47ae89.png)

input과 가중치를 summation한 값이 바로 출력되는 것이 아닌, activation function을 통과한 후 출력이 된다

![image](https://user-images.githubusercontent.com/107015573/215404223-cc114d00-5f95-495b-afbc-ea6fcfc195e9.png)

Hidden Units
- Activation function  
  - 들어오는 자극(data)가 크면 positive 값으로 활성화 시킨다- 비선형 transform[이를 위해 Activation function은 Sigmoid, tanh, ReLU를 사용]

### Output Layer에서 activation function의 역할
- class를 분류하는 역할(ex : 남자인가 여자인가, 암인가 아닌가, 아픈가 안아픈가)
![image](https://user-images.githubusercontent.com/107015573/215404399-1efaafe4-40ec-4ec4-9b72-f736d30c6bec.png)

- Output은 위에서 MLP 결과값을 본 것처럼 한다
- Sigmoid 사용했을 때 class 1,2가 있다 가정, 
- Sigmoid는 0과 1사이에서 bound된다. 2-1번클래스가 될 확률을 통해 클래스를 분류했다

Hidden에서는 정보가 얼마나 강하게 들어오는가를 판별해준다면(정보의 중요성) Output에서는 class를 구분하는 분류
