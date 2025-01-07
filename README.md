# <기부자 특성분석 및 예측>

* 데이터 : 한국보건사회연구원 한국복지패널 (https://www.koweps.re.kr:442/data/data/list.do)
* 데이터기간 : 2005년~2023년
* 분석대상(Y) : 지난 1년간 기부를 1만원 이상 하는지 여부
* 활용변수(X) : Y 변수를 제외한 나머지 변수
    * 전체 중에 50% 이상이 비어있는 변수는 삭제
    * 변수 값이 1개만 존재하는 변수는 삭제
    * 개인정보를 의미하는 ID 등의 변수는 삭제
    * 가중치 같은 필요없는 변수는 삭제
---
* 활용 알고리즘 후보 :
    * Machine Learning 5종: Logistic Regression, Random Forest, XGBoost, LGBM, CatBoost
    * Deep Learning 2종: Multi-Layer Perception (MLP), Convolutional Neural Network (CNN)
* 불균형 데이터 처리 방법 :
    * Downsample Negative Class
---
* XAI (Explainable AI) 분석:
   * SHAP (SHapley Additive exPlanations)을 활용하여 모델의 예측 결과를 해석
   * SHAP 값을 통해 각 변수의 기여도를 분석하고, 기부 여부 예측에 가장 큰 영향을 미치는 주요 변수를 식별
