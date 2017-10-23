# Introduction

## 1. Layer의 의미

![simple](http://i.imgur.com/z4gMY38.png)

- 위 이미지에서는 다음처럼 feature의 연결고리가 존재한다.
    + Size, bedrooms -> Family size
    + Zip code -> Walkability
    + Wealth -> School quality
- 레이어의 결과들이 모여서 마지막으로 price를 결정한다. 즉 패턴의 패턴을 찾는 것. CNN만 그런 것이 아니라 기본적인 MLP 구조의 의미가 그러하다.
- 하지만 실제로 Neural Networks를 만들 때 위처럼 인풋의 연결을 제한하지 않는다. Family size는 size와 bedrooms만 인풋으로 받지만 사용자가 제한하지 않는다는 것.
- 충분한 데이터를 넣으면 뉴럴넷이 알아서 이러한 연결도 알아낸다. 그래서 좋다는 것.

## 2. 데이터 증가, 컴퓨터 고성능화

![graphs](http://i.imgur.com/JhAEWM6.png)

- 과거의 알고리즘들은 데이터가 어느 수준 이상으로 커지면 성능이 좋아지지 않는다.
- 이론상으로 충분한 데이터와 충분한 parameter가 주어진다면 Multilayer perceptron은 모든 함수를 근사할 수 있다. 그래서 위처럼 데이터를 많이 넣어주면 성능이 계속해서 증가한다.
- 하지만 데이터가 적을 때는 좀 더 알고리즘 자체와 엔지니어의 역량이 중요해져서 뉴럴넷보다 기존 알고리즘이 더 성능이 잘 나올 수 있다.
