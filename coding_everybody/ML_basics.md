# 생활코딩 machine_Learning1(정리)

##### 결정 = 비교 + 선택
 	비교: 쉽지 않으면 결정이 어려워짐.
 	수: 비교를 위한 가장 중요한 수단
 	수 -> 통계 -> 결정능력 up
 	결정을 기계에 (스스로 결정) => 기계학습

##### Model
	현상 -> 추측 => 가설 -> 모순(x) => 이론
	판단력 =>> 모델, 모델을 만드는 과정 => 학습

##### Data
	Data Science: data를 만들고 이용
	Data Engineering: data를 다루는 도구를 만듬

##### 표
	행(row): 개체(instance), 관측치(observed value), 기록(record), 사례(example), 경우(case)
	열(column): 특성(feature), 속성(attribute), 변수(variable), field



##### 독립변수, 종속변수
	독립변수: 결과에 영향을 받지않는 독립적인 사건, 원인
	종속변수: 원인에 종속, 결과
	한쪽의 값이 바뀌었을때 다른쪽 값이 바뀌면 2개의 특성은 관련이 있다고 추측 가능. 이 때 2개의 특성은 서로 상관에 있다. => 상관관계
	각 열이 원인과 결과의 관계일 때 2개의 열은 "인과관계"
	독립변수와 종속변수는 인과관계		*[상관관계 >= 인과관계]*

##### 머신러닝의 분류
	기계학습(Machine Learning): 지도학습, 비지도학습, 강화학습
	- 지도학습(Supervised Learning): 분류, 회귀
		-지도학습 => 기계를 가르침(문제, 정답), data로 컴퓨터를 학습 => 모델을 생성
	- 비지도학습(Unsupervised Learning): 군집화, 변환, 연관
		-비지도학습 => 지도학습에 포함(x), 기계에게 data에 대한 통찰력을 부여, 관찰을 통해 새로운 의미, 관계를 찾음.
	- 강화학습(reinforcement Learning): 학습을 통해 능력을 향상시킨다는 점에서는 지도학습과 비슷
		- 차이점: 어떻게 하면 능력을 향상?, 기계 스스로가 반복(능력향상)

##### 지도학습
	과거의 data로 부터 학습, 결과를 예측
	과거의 data 필요 => 독립변수와 종속변수로 분리 => 이 관계를 컴퓨터에게 학습
	공식을 만듬 (공식 -> 모델)	*data가 많고 정확도가 높으면 좋은 모델*
	
##### 회귀(Regression)
	보통 예측하고 싶은 종속변수가 숫자일때 보통 회귀를 이용!

##### 분류(Classification)
	성격에 맞게 grouping
		Input			  Output	
	ex) 손톱사진: 독립변수 -> 손톱: 종속변수
		정상사진: 독립변수 -> 정상: 종속변수
		*결과가 숫자X, 결과-> 이름,문자*

##### 군집화(Clustering)
	비슷한 것들을 찾아서 group을 만드는 것
	 *군집화 vs 분류
		군집화: 비슷한 것들 끼리 모아서 적당한 group 만들기
		분류: 각각의 물건을 적당한 group에 위치시킴, 어떤 대상이 어떤 group에 속하는지?

##### 연관규칙학습(Association rule learning)
	장바구니 학습 ex) 라면을 구임한 사람은 계란도 구입
	과거에는 보통 추천시스템에 많이 사용, 최근에는 추천시스템에 다양한 방법을 사용
	관련이 있는 특성, 열을 찾아줌
	*관측치를 grouping => 군집화
	*특성을 grouping => 연관규칙

##### 변환(Transform)
	data를 새롭게 표현, 분석가 또는 다른 머신러닝 알고리즘이 원본데이터에 비해 쉽게 data를 해석할 수 있도록 만드는 과정
	ex) 차원축소: 특성이 많은 고차원 데이터의 특성의 수를 줄이면서 필요한 특징만 포함 *(시각화를 위해 2차원으로 보통 변환)

##### 지도, 비지도 정리
	비지도학습: 탐험적, data들의 성격을 파악하는 것이 목적
	지도학습: 역사적, 과거의 원인과 결과를 바탕으로 결과를 모르는 원인이 발생했을때 어떠한 결과가 나올지 추측 *(독립변수, 종속변수 중요!)
	
##### 강화학습(Reinforcement learning)
	지도학습: 배움을 통해 실력 up
	강화학습: 경험을 통해 실력 up
	*강화학습: 상태(state)에 따라서 더 많은 보상(reward)을 받을 수 있는 행동(action)을 에이전트(agent)가 할 수 있도록 하는 정책(policy)을 만드는 것이 목적