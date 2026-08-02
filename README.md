# 데이터 분석 실습

엔코아 AI캠퍼스 · 데이터 분석 & AI 머신러닝 캠프 실습 저장소입니다.

## 프로젝트

### [커머스] H&M 고객·매출 데이터 분석

Kaggle H&M Personalized Fashion Recommendations 표본(2019년 1년치)으로
문제 정의부터 인사이트 도출까지 전 과정을 수행한 종합 실습입니다.

| 노트북 | 내용 |
| --- | --- |
| `01_데이터이해_전처리.ipynb` | 문제 정의 · 데이터 품질 진단 · 전처리 규칙 수립 및 적용 |
| `02_데이터_EDA.ipynb` | 기술통계 · 집계 비교분석 · 시각화 |
| `03_데이터_통계.ipynb` | 가설검정 · 최종 인사이트 리포트 |

**분석 목표** — 마케팅팀의 타깃 프로모션 전략 수립을 위해 채널·연령대·시기별
결제금액 패턴을 파악한다.

**데이터** — 거래 150,500행 · 고객 95,516행 · 상품 30,503행을 결합 후
정제해 114,544행으로 분석했습니다.

**주요 발견**
- 온라인 평균 단가가 오프라인의 1.31배이나 효과크기는 작은~중간 수준(Cohen's d = 0.371)
- 연령대별 단가 차이는 유의하지만 실질적 크기가 거의 없음(η² = 0.0037)
- 가입 대기(PRE-CREATE) 고객의 구매 99.9%가 온라인에서 발생
- 6월은 거래 건수가, 9·11월은 단가가 매출을 견인

**한계** — Kaggle 공개 표본이라 전체 고객으로 일반화할 수 없고, `price`는
정규화된 상대값이며 수량 컬럼이 없어 합계는 매출이 아닌 "구매 단가의 총합"입니다.
관찰 데이터이므로 인과 해석은 불가능합니다.

## 환경

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?logo=python&logoColor=white)
![seaborn](https://img.shields.io/badge/seaborn-4C8CBF)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?logo=scipy&logoColor=white)
![pingouin](https://img.shields.io/badge/pingouin-5B8C5A)
![statsmodels](https://img.shields.io/badge/statsmodels-3B6E8F)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

## 실행 순서

`01` → `02` → `03` 순서로 실행합니다. `01`이 저장하는 정제본을 `02`·`03`이 이어받습니다.
원본 CSV는 저장소에 포함되어 있지 않습니다.
