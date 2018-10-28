[TOC]

# DS School 입문반 Week 3

## Decision Tree Concept

### Fit

| features    | label    |
| ----------- | -------- |
| sex         | Survived |
| pclass      |          |
| Embarked... |          |

### Gini Impurity

$$
{1 - (P_{survived}) ^ 2}  - {(P_{perish}) ^ 2} \\ 
\text{Generalized to} \\
{1 - (P_{label})^2 - {(P_{featur_n})^2}} \\
\text{until 0 or doesn't converge or reach to max_depth}
$$

### Data Visualization



### 데이터 분석 팁

- EDA를 먼저 (툴은 무방, 엑셀도 좋다)
- Kaggle Discussion 참고
- 데이터와 Feature를 많이 넣을 수록 점수가 오른다 (일반적으로)
- 역효과가 나는 Feature는 과감히 뺀다
- Encoding 활용

### Bike Sharing Demand Plan

- Datetime <- 연, 월, 일로 쪼개기
  - 데이터는 19일까지 밖에 없는데???
  - 20일부터는 Test 데이터 셋에 있음. 따라서 연/월/시간 만 의미 있을 듯
- Season <- Encode
  - 1 <- 겨울
  - 2 <- 봄
  - 3 <- 여름
  - 4 <- 가을
- Working day + Holiday = 0는 일하지 않는 날
  - nonworkingday
  - 굳이 Encoding하지 않아도 되지 않음?
- weather <- Encode
  - 1 <- pleasant
  - 2 <- mild
  - 3 <- light
  - 4 <- heavy
- temp and atemp gap <- Investigate
- temp 와 count 상관 관계 (특정 구간에서 떨어지는 일은 없는지)
- atemp와 count 상관 관계 (특정 구간에서 높아지고 떨어지는 일은 없는지)
- humidity
- Windspeed 미 계측값 처리

