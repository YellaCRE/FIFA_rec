# FIFA_Recommend System


### FIFA_crawling

피파온라인4 OpenAPI를 이용한 선수 스크래핑
https://developers.nexon.com/fifaonline4

### FIFA_EDA

기본통계값 EDA와 포지션별 데이터 세분화 및 분석

### FIFA_preprocess

기본 전처리 및 강화를 적용한 Data transformation

### FIFA_modeling

입력 받은 선수를 기반으로 컨텐츠기반 필터링을 활용하여 최적의 선수를 검색

피파온라인4 게임의 특성을 반영하여 능력치의 경우 하한점을 설정하여 그 이상인 선수들만 추천되도록 설계되었지만,  
[키, 몸무게, 체형] 같은 수치의 경우 하한점이 아닌 입력값과 유사한 선수일수록 추천점수가 높게 설정.  
이는 [키, 몸무게, 체형]의 경우 수치가 높을수록 우수한 성능을 보이는 것이 아닌 '체감'이라는 수치이외의 성능에 영향을 주기 때문에 위와 같이 설정함.


# Results

사용자가 입력한 선수 4명을 받았을 때 도출되는 결과 예시

<img width="485" alt="image" src="https://user-images.githubusercontent.com/76480887/220229512-c768d9b3-3d53-4477-8f1b-6602b7410df3.png">

입력 받은 선수들을 분석하여 우선순위에 따라 선수 추천  
피파온라인4 유저들에게 테스트모델 배포결과 긍정적인 피드백을 받음.
