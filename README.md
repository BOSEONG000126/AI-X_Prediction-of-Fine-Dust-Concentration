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


### 데이터 전처리
* ***사용 언어: jupyter python***
* [데이터 전처리 코드](https://github.com/soycong/HealthCure/tree/main/DataAnalysis)
![image](https://user-images.githubusercontent.com/62353647/202632808-ecc87a19-67c6-46ff-bfaa-5dd563a865d3.png)  

<br/>

## Data Analysis
### [1] 데이터 셋의 기본 변수 확인하기
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/a179c2dc-9a2a-4954-b159-9cab67a3dc51"  width="700" height="250">

  + EDA한 dataset의 instance의 수는 5881개 입니다.
  + Lable은 Laying, Standing, Sitting, Walking, Walking_upstairs, Walking_downstairs로 총 6개의 Lable을 가집니다.
  + 가속 센서, 자이로 센서, 각센서에서 특정 기준으로 측정되는 값을 다양한 방식으로 가공한 값을 Feature로 사용하고 있습니다.
<br/>

### [2] 단변량 , 이변량 EDA 진행
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/c05ec430-38dc-4afb-815b-d9d934aa274e" width="700" height="350">

  + 각 특징 데이터의 분석을 통하여 각기 행동을 분류할 feature 추출합니다.
<br/>

### [3] 단계별 모델링
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/8287f4fd-a5d9-4c59-9e70-436aaa088351" width="700" height="350">

 + 특징 분류 feature를 이용하여 정적 행동 , 동적 행동을 구분하는 모델 생성합니다.
 + Random Forest , XGboost , SVM , KNN 등 다양한 모델으로 데이터 분할 및 학습 후 가장 성능이 좋은 모델을 선정합니다.
<br/>

### [4] 분류 모델 합치기
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/c7e357eb-6123-4a33-bfbf-485743dda527" width="700" height="350">

 + 두 단계 모델을 통합하고, 새로운 데이터(test)에 대해서 최종 예측결과와 성능평가가 나오도록 함수로 만듦니다.
 + 데이터 파이프라인 구축 : test데이터가 로딩되어 전처리 과정을 거치고, 예측 및 성능 평가 수행합니다.
<br/>

## 활용

### [1] 서비스 컨셉
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/0c072553-565d-411b-aef8-5e7ceb4c531a" width="700" height="400">

 + 반려견의 생활 패턴을 분석하여 견주에게 도움을 주고자 합니다.

<br/>

### [2] 기능
<img src="https://github.com/BOSEONG000126/AI-X_Project/assets/116350240/a6c1cb14-e5b1-46b7-8cfc-869ad24fab83" width="700" height="400">

  + 활동량 체크
  + 휴식량 체크
  + 분리불안 감지
  + 수면 패턴 분석
<br/>

### [3] 기대효과
 + 반려견과 견주들간의 의사소통 편리
 + 반려견의 스트레스 감소
 + 견주와 반려견 사이의 유대감 증가
