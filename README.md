# **도서관 이용률과 정신 건강의 상관관계 분석**
- 2024 도서관 빅데이터 활용 및 아이디어 공모전 (2인 팀 프로젝트)

<br>

## 분석 배경
- 다양한 양상의 **정신 질환**이 현대인들의 **골칫거리**가 되고 있음.
    - 국가 정신건강현황 보고서 2022에 따르면, 대한민국 국민 4명 중 한 명은 평생 한 번 이상 정신질환을 겪고 있음.
    - 정신 질환은 개인의 삶의 질 저하는 물론이고, **사회적 비용 증가**를 초래함으로써 막대한 피해를 끼침.

<br>

- 도서관이 현대인의 **정신건강**을 위한 정보 제공 및 지원의 역할을 **충분히 수행하지 못하고 있음.**
    - 도서관은 단순히 책을 대출하는 공간을 넘어, 다양한 정보와 지식을 제공하며 지역 사회의 문화적 중심지로서 기능함.
    - 노영희, 오상희(2011)에 따르면, 공공도서관 이용자의 약 60%가 도서관에서 소비자 건강정보(CHI)를 제공할 필요가 있다고 생각했으나, 실제로 이러한 서비스를 제공하는 공공도서관은 **약 17.25%에 그쳤음.**

<br>

## 문제 정의
- **정신질환 심각도**와 **도서관 이용 지표** 간의 관계를 시군구별로 확인
- 분석 결과를 토대로, **정신건강 개선**을 위한 도서관의 역할과 기여 방안을 제안

<br>

## 분석 내용
- 시군구별 **정신질환 심각도**를 파악함.
    - 건강보험심사평가원의 제공 데이터를 기반으로 주요 정신질환 4종을 정의함.
    - 정의된 4가지 정신질환의 발병률을 기반으로, 행정구별 정신질환 심각도를 도출함.
        - 주민등록 **인구 수** 대비 정신질환 **환자의 비율**을 산출한 뒤 정규화하여 **Z-Score**를 계산함.

<br>

- 정신질환 심각도와 **도서관 요인**의 관계를 확인함.
    - 정신질환 심각도가 도서관 규모 및 이용률과 관련이 있는지 알아보기 위해 **다중회귀분석**을 수행함.
    - **회귀계수**의 통계적 유의성을 확인하여, 도서관 요인 중 정신질환 심각도에 영향을 끼치는 변수를 식별함.

<br>

- 정신질환 및 도서관 요인의 데이터 유사성을 기반으로 **클러스터링**을 수행함.
    - 회귀계수 기반 **변수 선택** 기법을 적용하여 input feature를 정의함.
    - Elbow Method를 활용하여 군집의 개수를 선택한 뒤, **K-Means 클러스터링**을 수행함.
    - 각 군집의 특성을 **정규분포 기반**으로 식별하여, 도서관 요인 및 정신질환 요인의 **분포 패턴**을 확인함.

<br>
 
## 결과 해석 및 활용 방안 제안
- 도서관이 **정신건강 증진**에 효과적으로 **기능하지 못하고 있음**을 파악하였음.
    - 정신질환 심각도가 높은 지역은 전반적으로 도서관 이용률이 높았음.
    - 정신질환 심각도가 낮은 지역은 대개 도서관 이용률이 낮은 편이었음.

<br>

- 도서관 자원을 활용한 **정신건강 개선 프로세스**의 개발이 필요함.
    - 공공도서관을 통한 정신건강 개선 정책 및 프로그램 수행을 제안함.
    - 정신질환 심각도가 높은 지역에서는 모바일 웹 접속 건수 또한 많았으므로, **모바일 웹**을 적극적으로 활용할 것을 제안함.

<br>
 
## References
- 노영희, 오상희. (2011). **"공공도서관의 소비자건강정보서비스에 대한 이용자인식 조사연구."** *한국도서관정보학회지, 42(3), 45-77.*
- 보건복지부. (2023). **"국가 정신건강현황 보고서 2022".**
