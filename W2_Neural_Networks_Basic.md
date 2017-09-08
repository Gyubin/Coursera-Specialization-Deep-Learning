# Neural Networks Basic

- logistic regression에서 마지막 output 내는 뉴런은 sigmoid를 쓴다.
- 항상 기본 꼴은 `WTX + b` 꼴이다.
    + X는 n by m 매트릭스: n은 feature 개수, m은 데이터 개수를 나타낸다.
    + 즉 row가 feature, column이 data example을 나타낸다.
    + X 우측 상단에 `(i)`라고 적히는 것은 i번째 example을 뜻함
- logistic regression
    + `y_hat = p(y = 1 | x)` 을 구하는 것
    + `z = wTx + b`
    + `a = sigmoid(z)` : 0과 1 사이의 값(확률 의미)으로 바꿈. 0.5를 기준으로 클래스 구분
- logistic regression cost
    + Maximum Likelihood Estimation을 사용
    + `ylog(y_hat) + (1-y)log(1-y_hat)`의 값을 최대화하는 parameter를 찾는 것이 목표
    + 일반적으로 최적화는 최소값을 구하는 것이라서 위 식에 마이너스를 붙여서 최소화해야할 cost로 만든다. `-(ylog(y_hat) + (1-y)log(1-y_hat))`
    + 데이터가 m개가 있을 때는 위 식의 `y`와 `y_hat`이  각각의 데이터가 되고 전체항을 `m`으로 나눠줘야함
- Gradient Descent
    - `w = w - alpha * dw`
    - `b = b - alpha * db`
