# Bank-marketing-campaign
통계분석실습 Project

## 1. 프로젝트 소개
한 은행에서 은행의 특정 상품을 홍보하여 예금을 수신하기 위해 은행의 고객들을 전화로 contact한 것과 연관된 자료.
이 자료를 활용하여 현재 진행하는 상품홍보에 적절한 telemarketing 전략을 수립하는 것이 project의 목표
- 고객들에게 선택적으로 telemarketing하는 것을 가정(거절할 것 같은 고객은 보류, 예금하기로 결정할 것 같은 고객에 대해서만 연락)하여 다음과 같이 classification을 하는 learner를 개발
  - marketing시 예금하기로 결정할 것 같은 고객 => telemarketing을 시도
  - marketing을 거절할 것 같은 고객 => telemarketing을 보류
  
- Performance Measure

  - 새로운 평가지표 개발의 이유: 은행은 자금의 합리적인 운용을 위해 기회비용과 손실을 고려하여 홍보전략을 수립해야됨.
  - telemarketing을 시도할 때의 비용을 –1, marketing에 성공했을 때의 이윤을 +6, marketing에 
실패했을 때 손해를 –1로, marketing을 시도했을 때 성공할 수 있는 고객을 marketing을 보류하여 
놓치는 기회비용을 –3으로 계산하여 총창출된 이윤(profit)을 learner의 performance measure로 함 

## 2. 데이터 설명

- Input variables

  - 고객과 관련된 정보: Age, Job, Marital, Education, Default, Housing, Loan
  - 현재 진행하고 있는 telemarketing에 대한 정보 : Contact, Month, Day_of_week
  - 기타 정보들: Campaign, Pdays, Previous, Poutcome
  - 사회 경제적 변수들 : emp.var.rate(고용변동율), cons.price.idx(소비자물가지수), cons.conf.idx(소비자신뢰지수)

- Output variable:

  - 고객이 은행에 예금을 예치했는지 여부 (yes/no)
    
## 3. Modeling
- Logistic Regression
- Random Forest
- XGBoost

## 4. 개발환경
- Python
