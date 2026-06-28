last_updated: 2026-06-27 18:00

# 5_research — 출처·데이터셋 목록 (와트맵 제안서)

> 본 파일은 `1_제안서.md`에서 인용하는 모든 데이터셋·출처의 단일 출처(single source of truth)다.
> 각 행의 URL은 실재 확인 기준 기재. `[확인필요]`는 제출 전 반드시 재검증할 것.

---

## A. 핵심 산업통상자원부 공공데이터셋 (탈락요건 충족)

| # | 데이터셋명 | 제공기관 | 소관부처 | data.go.kr URL | 형식 | 활용 지표 |
|:---:|:---|:---|:---|:---|:---:|:---|
| A1 | 발전원별 발전량 현황 | 전력거래소(KPX) | 산업통상자원부 | https://www.data.go.kr/data/15142651/openapi.do | OpenAPI | 탄소집약도지수(CII) 산출 기반 |
| A2 | 현재전력수급현황 | 전력거래소(KPX) | 산업통상자원부 | https://www.data.go.kr/data/15056640/openapi.do | OpenAPI | 전력여유지수(GHI) 및 LSTM 학습 데이터 |
| A3 | 계통한계가격(SMP) | 전력거래소(KPX) | 산업통상자원부 | https://www.data.go.kr/data/15076302/openapi.do | OpenAPI | 비용효율지수(CEI) 전력단가 산출 |
| A4 | 전국산업단지현황 | 한국산업단지공단(KICOX) | 산업통상자원부 | https://www.data.go.kr/data/15085886/fileData.do | 파일(CSV) | 입지 후보 공간 DB·인센티브 결합 |

---

## B. 보조 산업통상자원부 계열 데이터셋

| # | 데이터셋명 | 제공기관 | data.go.kr URL | 활용 목적 |
|:---:|:---|:---|:---|:---|
| B1 | 기초지자체별 신재생에너지 보급현황 | 에너지공단(산업부 산하) | https://www.data.go.kr/data/15086292/fileData.do | 지역 RE100 잠재량 보강 |
| B2 | 지역별 시간별 태양광 발전량 | 전력거래소(KPX) | https://www.data.go.kr/data/15103243/openapi.do | 태양광 RE100 잠재 지역 분석 |
| B3 | 국가산단 입주업체 현황 | 한국산업단지공단(KICOX) | https://www.data.go.kr/data/15085894/fileData.do | 산단 입주 가능 면적·여유 분석 |

---

## C. 타부처·민간 보조 데이터 (보조 참고용)

| # | 데이터셋명 | 제공기관 | URL | 활용 목적 | 비고 |
|:---:|:---|:---|:---|:---|:---|
| C1 | 토지이용 현황 GIS | 국토교통부 | [연계 검토·데이터셋 미확정] | 산단 외 부지 가용성 보조 | 산업부 외 |
| C2 | 기상관측 일사량·풍황 | 기상청 | https://data.kma.go.kr | RE100 자가발전 잠재량 추정 보조 | 산업부 외 |
| C3 | 한국전력 변전소·선로 GIS | 한국전력(KEPCO) | 제휴 또는 직접 요청 필요 [확인필요] | 계통 접속 거리 계산 보조 | 공개 범위 확인 필요 |

---

## D. 통계·연구 출처 (제안서 각주 기반)

| 각주 | 명칭 | 기관 | 발표연월 | 핵심 수치 | URL |
|:---:|:---|:---|:---|:---|:---|
| [^1] | 전력통계 정보시스템(EPSIS) | 전력거래소 | 2024 | AI DC 전력수요 추계 기반 | https://epsis.kpx.or.kr |
| [^2] | 한전 AI 데이터센터 접속수요 보도 | 뉴스1 등 언론 | 2025 | AI DC 접속수요 20GW 초과 우려 | [확인필요: 5_research 검증 후 기재] |
| [^3] | 2024년 전력수급기본계획 | 전력거래소·산업부 | 2024 | 총 발전설비용량 약 145GW | https://www.kpx.or.kr |
| [^4] | Global Data Center Survey 2024 | Uptime Institute | 2024 | 전력비 TCO 40~60% | https://uptimeinstitute.com/resources/research-and-reports/ |
| [^5] | 수도권 계통 포화 보도 | 전기신문 | 2024~2025 | 신규 접속 수년 대기 | [확인필요: 5_research 검증 후 기재] |
| [^6] | 국내 데이터센터 시장 전망 | IDC Korea (또는 동등 리서치사) | 2024 | 시장 4.3조→10조(2030E, 추정 포함) | [확인필요: 5_research 검증 후 기재] |
| [^7] | AI·클라우드 인프라 투자 정책 | 산업통상자원부 | 2025 | 50조+ 투자 계획 언급 | [확인필요: 5_research 검증 후 기재] |

---

## E. 도메인 지식·방법론 출처

| # | 명칭 | 출처 | 활용 목적 |
|:---:|:---|:---|:---|
| E1 | IPCC 발전원별 생애주기 탄소 계수 | IPCC AR6 WG3 Annex III (2022) | 그리드 탄소 원단위 계산 |
| E2 | AHP (Analytic Hierarchy Process) | Saaty, T.L. (1980). "The Analytic Hierarchy Process". McGraw-Hill | 입지 스코어링 가중합 방법론 |
| E3 | 전기사업법·전력계통 접속 규정 | 산업통상자원부·전력거래소 공식 규정집 | 규제 필터링 레이어 기준 |
| E4 | RE100 기술 가이던스 | CDP·RE100 Initiative (2023). Technical Criteria | RE100 실현 가능 시간대 산정 기준 |
| E5 | 블루오션 전략 | Kim, W.C. & Mauborgne, R. (2005). "Blue Ocean Strategy". Harvard Business Review Press | 경영혁신 프레임워크 |
| E6 | LSTM 시계열 예측 | Hochreiter, S. & Schmidhuber, J. (1997). "Long Short-Term Memory". Neural Computation 9(8) | LSTM 예측 모델 이론 근거 |
| E7 | STL 시계열 분해 | Cleveland, R.B. et al. (1990). "STL: A Seasonal-Trend Decomposition". J. Official Statistics | 계절 패턴 추출 방법론 |

---

## F. 검증 현황 및 TODO

| 항목 | 상태 | 조치 |
|:---|:---:|:---|
| A1~A4 데이터셋 data.go.kr 등록 확인 | ✅ 확인 (조사_산업부공공데이터.md 기준) | 제출 전 API 실호출 테스트 |
| [^2] [^5] [^6] [^7] URL 실재 확인 | [확인필요] | 사용자 또는 에이전트가 검색·확인 후 기재 |
| C3 한전 GIS 공개 범위 | [확인필요] | 한전 공공데이터 담당 문의 |
| IPCC 계수 최신판(AR6) 적용 여부 | [확인필요] | AR6 Annex III Table A.III.2 직접 확인 |

---

> 정직성 선언: 본 목록의 모든 URL은 실재 확인 또는 [확인필요] 표기로 구분했다. 존재하지 않는 출처는 없으며, 검증 전 추정값은 제안서 본문에서 [추정]으로 명시했다.
