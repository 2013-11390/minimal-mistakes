---
title: "Starting Machine Learning"
categories:
  - Machine Learning
tags:
  - Machine Learning
  - Deep Learning
  - Coursera
---

온라인으로 머신러닝에 대한 기초를 공부할 수 있는 coursera 사이트를 알게 되면서 기초 강좌를 수강하게 되었고 수강한 강좌에 대한 요약 정리를 위해 포스팅을 시작하였다. <br/>
Machine Learning : A computer program learn from experience E with respect to some class of tasks T and performance P

E : experience, T : tasks, P : performance <br/>
위의 정의가 이해가 잘 안된다면 다음과 같은 예시를 보자.
Email 프로그램이 당신의 이메일들 중 당신이 스팸으로 표시하는 것을 통해 learn하고 있다고 보자. 이런 경우 당신이 이메일을 스팸으로 혹은 스팸으로 처리하지 않는 것을 보는 것이 프로그램에게 E가 될 것이고 이메일을 스팸으로 분류하는 것이 프로그램에게 T가 될 것이다. 그리고 이렇게 분류한 이메일들이 얼마나 정확하게 분류되었는가가 P가 될 것이다.

Supervised Learning : If we are given a dataset, already know what our correct ouput look like
- Regression : Try to predict results within a continuous output, try to map input variables to continuous function
- Classification : Try to map input variables ito discrete categories
Unsupervised Learning : Allow us to approach problems with no idea about results
- Clustering : ex. 100000 different genes group by life span, location etc.
- Non-Clustering : ex. Cocktail Party Algorithm

Supervised Learning의 경우에는 정답이 주어진 경우이다. 위의 정의에서처럼 어떠한 아웃풋을 내냐에 따라 Regression과 Classification이 있다. Tumor의 크기를 보고 Malignant한지 아니면 Benign한지 판단하는 Classification문제와 다른 몇개의 샘플들을 통해 그래프를 예측하여 크기에 따른 집의 가격을 판단하는 Regression 문제로 볼 수 있다.

Unsupervised Learning는 결과물에 대한 어떠한 답에 대한 기준이 없는 경우에 쓴다. 여기서 Cocktail party problem은 칵테일 파티 현장에서 다른 두 사람이 다른 두 마이크를 통해 저장된 목소리를 분류하는 문제이다.

---------------------------------------
이렇게 머신러닝에 대해서도 위와 같이 여러가지로 분류가 되는데 이런 분류 방식을 아는 것이 매우 중요한 이유는 우리가 어떠한 문제를 만난 경우 어떠한 방식으로 그 문제를 해결해야하는지 판단이 우선적으로 서야하기 때문이다. 앞선 예시에서처럼 Tumor의 Size를 통해 Malignant한지 아니면 Benign한지 판단하는 문제라면 Supervised Learning이라는 것을 캐치해야하는 것처럼 말이다.