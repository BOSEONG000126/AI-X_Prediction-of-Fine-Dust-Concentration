# AI+X 미세먼지농도 예측 Project
<img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/bdda3b35-7193-454b-93e2-f41055421ebf" width="1000" height="300">

<br/>

---
## 활용 데이터셋
### [1] 미세먼지 및 오염물질 정보 (에어코리아)
<img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/561a66ab-ef88-47aa-84b9-6553f98af6e9" width="800" height="400">
* [데이터셋 출처 링크](https://www.airkorea.or.kr/web/pastSearch?pMENU_NO=123)
<br/>

### [2] 날씨 정보 (기상청)
<img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/d093f226-a0e9-4c05-8dad-9a2a2c31e6f2" width="800" height="400">
* [데이터셋 출처 링크](https://www.airkorea.or.kr/web/pastSearch?pMENU_NO=123)

<br/>

## Data Engineering
### [1] Data Analysis
<img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/16ad4cbb-0b91-4760-a994-4bf86a33cecb"  width="400" height="250"> <img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/954d37a6-423b-4419-af5c-fe2aafec9f7d"  width="400" height="250">

  + 미세먼지가 100 이하일때는 다른 먼지 co , no2 ,초미세먼지 등 다른먼지와 PM10은 양의 상관계수가 나옴.
  + 하지만 미세먼지가 100 이상일때 다른 먼지 co , no2 , 초미세먼지와 PM10은 음의 상관게수가 나옴.
<br/>

### [2] Data 전처리
<img src="https://github.com/BOSEONG000126/AI-X_Prediction-of-Fine-Dust-Concentration/assets/116350240/bf27b866-1daf-4d90-a225-5d5f095ee852" width="700" height="350">

  + 학습에 필요한 Feature 생성 , 필요없는 Feature 삭제
  + 결측치가 1000개 이상인 Feature 삭제
<br/>

### [3] ML Modeling
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/8287f4fd-a5d9-4c59-9e70-436aaa088351" width="700" height="350">

 + 특징 분류 feature를 이용하여 정적 행동 , 동적 행동을 구분하는 모델 생성합니다.
 + Random Forest , XGboost , SVM , KNN 등 다양한 모델으로 데이터 분할 및 학습 후 가장 성능이 좋은 모델을 선정합니다.
<br/>
