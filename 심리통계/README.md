# Psychological Statistics
성격 특성 기반 고객 타겟팅 전략 : Big5 성격 요인과 FoMO를 기반으로 한 영화 제작 접근법

## EDA 프로젝트 자료 소개
> * Dataset 
>   * [dataset]()
> * [EDA 발표자료](): 프로젝트 내용을 정리한 발표 자료입니다.
> * [EDA 최종 코드]() : EDA 발표와 관련하여 사용된 코드입니다.

## 🖥️ 프로젝트 소개
심리학에서 널리 쓰이는 'Big Five' 성격 특성 이론과 Fear of Missing Out(FoMO) 경향을 활용해, 높은 입소문 효과를 가져올 수 있는 영화 장르/특성을 추출한 프로젝트입니다.
<br>

### 👑 프로젝트 멤버
- 백두형(팀장), 김여원, 복지민, 이정우
### 🕰️ 개발 기간
* 24.07.09 - 24.08.06

## 📒 구현 사항
#### Big5 특성에 따른 관객군 클러스터링 
- UMAP 차원축소
- Gaussian Mixture Model 클러스터링
- Daveis-Bouldin Index와 Calinski-Harabasz Index를 통해 최적 클러스터 탐색
#### Aspect-Based Sentiment Analysis(ABSA)를 활용한 영화 특성 추출
- IMDB 사이트에서 Total Votes가 가장 높은 리뷰 Top 3 크롤링
- Longformer 모델을 이용한 리뷰 요약
- GPT API를 활용한 ABSA 수행
- spaCy를 이용하여 리뷰에서 추출한 태그 중 공통 태그만 분리
#### 결론 도출
- Z분석을 통한 '입소문 관객' 선호 태그, 비선호 태그 발견
