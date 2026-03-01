# 📒 Week 1: Statistical Estimation (MLE & MAP)

---

## 1. 기계학습의 정의 (Definition of Machine Learning)
[cite_start]기계학습은 컴퓨터 프로그램이 경험(E)으로부터 학습하여, 특정 작업(T)을 수행할 때 성능(P)이 향상되는 것을 의미합니다. 

* [cite_start]**Experience (E)**: 관측된 데이터셋 (예: 동전 던지기 결과) 
* [cite_start]**Task (T)**: 해결하고자 하는 문제 (예: 다음에 앞면이 나올지 예측) 
* [cite_start]**Performance (P)**: 모델의 정확도나 성능 측정 지표 

## 2. 최대 우도 추정 (Maximum Likelihood Estimation, MLE)
[cite_start]MLE는 관측된 데이터 $D$가 발생할 확률인 **우도(Likelihood)**를 최대화하는 파라미터 $\theta$를 찾는 빈도주의적 접근 방식입니다. 

* [cite_start]**Likelihood Function**: $L(\theta) = P(D|\theta)$ 
* **MLE의 목적 함수**:
$$\hat{\theta} = \text{argmax}_{\theta} \text{[P(D|\theta)]}$$
* [cite_start]**동전 던지기(Binomial)에서의 MLE**: 앞면이 $a_H$번, 뒷면이 $a_T$번 나왔을 때, 앞면이 나올 확률 $\hat{\theta}$은 **$\frac{a_H}{a_H + a_T}$** 입니다. 

## 3. 베이즈 정리와 MAP (Bayes' Theorem & MAP)
[cite_start]사전 지식(Prior)을 활용하여 데이터가 주어졌을 때의 사후 확률을 추정하는 방식입니다. 

* **Bayes' Theorem**:
$$P(\theta|D) = \frac{P(D|\theta)P(\theta)}{P(D)}$$
* [cite_start]**$P(\theta|D)$**: **[사후 확률]** (Posterior) 
* [cite_start]**$P(D|\theta)$**: **[우도]** (Likelihood) 
* [cite_start]**$P(\theta)$**: **[사전 확률]** (Prior Knowledge) 
* [cite_start]**$P(D)$**: **[정규화 상수]** (Normalizing Constant) 

* [cite_start]**MAP (Maximum A Posteriori)**: 사후 확률을 최대화하는 파라미터를 찾습니다. [cite: 3]
$$\hat{\theta}_{MAP} = \text{argmax}_{\theta} P(D|\theta)P(\theta)$$

# Probability Distribution (확률 분포) 요약

## 1. 확률 분포 개요 (Overview)
* **정의**: 무작위 시행, 실험, 설문 등의 잠재적 사건 부분집합에 확률을 할당함
* **기능**: 사건을 확률로 매핑하는 함수 (확률의 공리 준수 필요)
* **사건의 유형**:
    * **연속 수치 (Continuous numeric value)**: 측정되는 연속적인 데이터
    * **이산 범주 (Discrete categorical value)**: 분류되는 불연속적 데이터
* **주요 표현**:
    * **PDF (Probability Density Function)**: 확률 밀도 함수, $f(x)$
    * **CDF (Cumulative Distribution Function)**: 누적 분포 함수, $\int_{-\infty}^{x} f(x) dx$

---

## 2. 주요 확률 분포

### 정규 분포 (Normal Distribution)
* **특징**: 연속 수치 데이터에서 가장 흔히 관찰되는 분포
* **수식**: $f(x; \mu, \sigma) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
* **표기**: $N(\mu, \sigma^2)$
* **통계량**: 평균 $\mu$, 분산 $\sigma^2$

### 베타 분포 (Beta Distribution)
* **특징**: $[0, 1]$ 사이의 닫힌 구간을 가지며, 확률의 특성을 모델링하기 좋음
* **수식**: $f(\theta; \alpha, \beta) = \frac{\theta^{\alpha-1}(1-\theta)^{\beta-1}}{B(\alpha, \beta)}$
* **표기**: $\text{Beta}(\alpha, \beta)$
* **통계량**: 평균 $\frac{\alpha}{\alpha+\beta}$, 분산 $\frac{\alpha\beta}{(\alpha+\beta)^2(\alpha+\beta+1)}$

### 이항 분포 (Binomial Distribution)
* **특징**: 이산형 값을 위한 가장 단순한 분포 (베르누이 시행: 0 또는 1)
* **수식**: $f(\theta; n, p) = \binom{n}{k} p^k (1-p)^{n-k}$
* **표기**: $B(n, p)$
* **통계량**: 평균 $np$, 분산 $np(1-p)$

### 다항 분포 (Multinomial Distribution)
* **특징**: 이항 분포의 일반화 (Yes/No를 넘어 여러 범주 선택 시 사용)
* **활용**: 단어 선택(Word selection), 클러스터 선택 모델링 등
* **수식**: $f(x_1, \dots, x_k; n, p_1, \dots, p_k) = \frac{n!}{x_1! \dots x_k!} p_1^{x_1} \dots p_k^{x_k}$
* **표기**: $\text{Mult}(P), P = <p_1, \dots, p_k>$
* **통계량**: 평균 $E(x_i) = np_i$, 분산 $\text{Var}(x_i) = np_i(1-p_i)$


## ✅ 정답 확인 (Answer Key)

<details>
<summary>여기를 눌러 정답을 확인하세요!</summary>

1. [cite_start]**$P(D|\theta)$** (또는 $L(\theta)$) 
2. [cite_start]**$\frac{a_H}{a_H + a_T}$** 
3. [cite_start]**사후 확률** (관측 후의 확률) 
4. [cite_start]**우도** (파라미터 조건 하의 데이터 확률) 
5. [cite_start]**사전 확률** (관측 전의 배경 지식) 
6. [cite_start]**베타(Beta)** 
7. [cite_start]**가상 관측치(Virtual counts)** 

</details>
