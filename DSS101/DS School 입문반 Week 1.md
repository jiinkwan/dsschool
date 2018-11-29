[TOC]

# DS School Week 1

## Kaggle

Data Science 경진 대회

기업, 정부, 기관 등에서 스폰서

4주간 목표 -> 상위권 진입

## Titanic

실제 데이터

Pessenger ID: 승객 고유 번호, 겹치는 부분이 없음

Survived: 0, 1 (Dead, Alive), only in training data.

Training 데이터를 통해 누가 죽었는지 살았는지에 대한 패턴을 찾고, Test 데이터를 통해 예측. 

pclass: 객실 등급

Sex: 성별

Age: 나이, Null 값이 있음. 어떻게 처리 할까?

Sibsp: Number of Sibling and Spouse.

Parch: Number of Parents and Children.

TIcket: Ticket 번호

Fare: 요금

Cabin: Cabin no

Embarked: 기항지. 

Train Data



Test Data



### They all died experiment

Assumming people all died.

- Accuracy: 0.62679
  - More people died than survived

### 데이터 분석 단계

가설 성립 -> 가설 검증 -> 예측

### Only women survived

Assumming only women survived

- Accuracy: 0.76076
  - More women survived than men

### Children has better off

If they are under 18, they will have better chance to survive.

- Actually it brought down the survival rate.
- Quantative column is difficult to handle with pivot table.

### Women in first and second class survive

0.75598

- Women in third class still has 50 percent of chance to survive
- Which dragged the whole score down

## Data Science with Python











# To-Do List

