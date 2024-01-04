# 2023년 광진구 빅데이터 분석 공모전
광진구의 평균 통행 속도는 서울특별시 25개 구 중 5위로 시내에서는 빠른 편에 속함

그러나 건대입구 부근의 경우 서울로 유입되는 동서남북의 교통량이 모이는 지점이며 고가도로까지 설치되어 있어 교통 정체 문제가 심각함

따라서 건대입구역 부근 교통 정체 해소를 통한 광진구민들의 삶의 질 향상이 절실함

이를 위해 광진구로 유입되는 주요 지점의 장소와 유입량을 기반으로 분석을 진행하여 교통 정체 해소 방안을 고안함

## 1. 광진구 교통정체 해소를 통한 광진구민 삶의 질 향상 대시보드
EDA를 위해 Tableau를 활용하여 대시보드를 제작, 본격적인 분석 전 교통 상황을 살펴봄
Tableau Public 링크 

: https://public.tableau.com/views/2023-Team/sheet0?:language=ko-KR&:display_count=n&:origin=viz_share_link
![건대입구역 실시간 교통 현황](https://github.com/lastdancewithyou/Gwangjingu_2023/assets/114273570/b9ca033e-2c2b-4ff0-bcb9-ca9aca8e2108)

## 2. 광진구 유출입 교통량에 따른 건대 입구 교통 속도 예측 모델링 & SHAP 활용 기여지점 판단
트리 기반 부스팅, 배깅 모델, 다층 퍼셉트론 모델, 선형 회귀 모델을 비교하였으며 Grid Search CV를 활용하여 모델별 최적의 하이퍼파라미터를 선정함

건대입구역 사거리로 향하는 8개의 출입 지점의 교통량을 모델에 넣은 결과 랜덤포레스트 RMSE가 가장 낮았고, 이를 SHAP 알고리즘에 적용함
<img width="1439" alt="스크린샷 2024-01-04 오전 10 24 15" src="https://github.com/lastdancewithyou/Gwangjingu_2023/assets/114273570/92b070c3-bc43-4357-88b7-0a9bf34f4f6a">

8개 지점에 모두 SHAP 알고리즘을 적용하고, 결과를 도출함

## 3. 결과 해석
도출된 차트들을 바탕으로 아래와 같이 결과를 해석함
<img width="1440" alt="스크린샷 2024-01-04 오전 10 27 53" src="https://github.com/lastdancewithyou/Gwangjingu_2023/assets/114273570/6c708c86-3337-4d8e-b872-7892cb8fdeed">

## 4. 정책 제안
최종적으로 광진구 교통 정체 해소를 위한 구체적인 정책을 제안함

1. 군자교 대체 교량 추가 건설
   
   1-1. 군자교 사거리 교통 체계 개선
<img width="1440" alt="스크린샷 2024-01-04 오전 10 28 11" src="https://github.com/lastdancewithyou/Gwangjingu_2023/assets/114273570/9981c8bf-ebfe-4d42-bc33-94c6aa0fd377">

2. 2호선 지하화
   
   2-1. 서울시의 재정 지원
   
   2-2. 횡단보도 지하화
<img width="1440" alt="스크린샷 2024-01-04 오전 10 28 19" src="https://github.com/lastdancewithyou/Gwangjingu_2023/assets/114273570/34733b24-96a8-43eb-a254-7fc617d13f43">
