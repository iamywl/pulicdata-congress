---
last_updated: 2026-06-27 15:00
프로젝트: 그린아워(GreenHour) — 실시간 탄소집약도 + 기업 RE100 조달 계산기
용도: 제안서(1_제안서.md) 인용 출처 통합 관리
---

# 5_research — 출처·데이터셋 목록

> 본 파일은 `1_제안서.md`의 각주(`[^번호]`)와 1:1로 연결되는 단일 출처 목록이다.
> 검증된 수치에만 출처를 기재하고, 추정값은 `[추정]`으로 별도 표기한다([`../CLAUDE.md` §2.6](../../CLAUDE.md) 준수).

---

## A. 핵심 공공데이터셋 (산업부 산하 — 탈락요건 충족)

| 번호 | 데이터셋명 | 제공기관 | 데이터 유형 | data.go.kr URL | 제안서 활용 |
|:---:|:---|:---|:---:|:---|:---|
| DS-01 | **발전원별 발전량 현황** | 전력거래소(KPX) — 산업통상자원부 산하 | API (실시간) | https://www.data.go.kr/data/15142651/openapi.do | 탄소집약도 엔진(CIE) 핵심 원천. 15분 단위 발전원별 발전량 → gCO₂/kWh 산출 |
| DS-02 | **기초지자체별 신재생에너지 보급 현황** | 한국에너지공단(KEA) — 산업통상자원부 산하 | 파일 (분기) | https://www.data.go.kr/data/15086292/fileData.do | 시군구 단위 신재생 설치용량 → 지역 PPA 조달 가능 용량 매핑(RRM 레이어) |

---

## B. 보조 공공데이터셋 (산업부 산하 — 보완 활용)

| 번호 | 데이터셋명 | 제공기관 | 데이터 유형 | URL | 제안서 활용 |
|:---:|:---|:---|:---:|:---|:---|
| DS-03 | 계통한계가격(SMP) | 전력거래소(KPX) | API | https://www.data.go.kr/data/15076302/openapi.do | PPA vs 시장가 경제성 비교 |
| DS-04 | 현재 전력수급현황 (5분) | 전력거래소(KPX) | API | https://www.data.go.kr/data/15056640/openapi.do | 실시간 예비율·수요 데이터(탄소집약도 보정) |
| DS-05 | 지역별 시간별 태양광 발전량 | 전력거래소(KPX) | API | https://www.data.go.kr/data/15103243/openapi.do | 태양광 패턴 학습 데이터 (LSTM 훈련용) |
| DS-06 | 산업분류별 전력사용량 | 한국전력(KEPCO) | API | https://www.data.go.kr/data/15101403/openapi.do | 업종별 벤치마크 탄소집약도 비교 |

---

## C. 타부처·민간 데이터 (보조 결합)

| 번호 | 데이터·보고서명 | 제공기관 | URL | 제안서 활용 |
|:---:|:---|:---|:---|:---|
| DS-07 | 배출권거래소 탄소배출권 거래내역 | 한국거래소(KRX) / 환경부 | https://ets.krx.co.kr | K-ETS REC·배출권 가격 시계열 |
| DS-08 | 국가 온실가스 인벤토리 보고서 | 온실가스종합정보센터(GIR) / 환경부 | https://www.gir.go.kr | 발전원별 배출계수(IPCC Tier 2) 검증 |
| DS-09 | K-ETS 3기(2026~2030) 계획 수립 방안 | 환경부 | https://www.me.go.kr | 무상할당 축소 일정 및 탄소비용 증가 전망 |
| DS-10 | CDP Korea Annual Report 2024 | CDP(Carbon Disclosure Project) | https://www.cdp.net/en/research/global-reports/korea | 국내 RE100 기업 조달률 12% 수치 [^1] |
| DS-11 | RE100 Annual Progress and Insights Report 2024 | RE100 / Climate Group | https://www.there100.org/re100-insights | 글로벌 평균 조달률 53%, 가입 438개사 [^2] |

---

## D. 학술·연구 문헌

| 각주 | 문헌명 | 저자/기관 | 연도 | URL / DOI | 핵심 인용 수치 |
|:---:|:---|:---|:---:|:---|:---|
| [^8] | Real-time carbon accounting method for the European electricity markets | Tranberg et al. | 2019 | https://doi.org/10.1016/j.esr.2019.100367 | 시간 단위 탄소집약도 기반 구매 → 탄소감축 15~30% 추가 효과 |
| [^10] | Carbon Management Software Market Report 2025 | MarketsandMarkets | 2025 | https://www.marketsandmarkets.com/Market-Reports/carbon-management-market.html | 시장 규모 $26억→$91억 (CAGR 28%) |

---

## E. 정부·기업 보도자료·공개 보고서

| 각주 | 자료명 | 기관 | 연도 | URL | 핵심 내용 |
|:---:|:---|:---|:---:|:---|:---|
| [^3] | 탄소국경조정제도(CBAM) 대응 전략 | 산업통상자원부 | 2025 | https://www.motie.go.kr | 국내 수출기업 CBAM 영향 분석 |
| [^4] | RE100 실행가이드 | 한국에너지공단 | 2024 | https://www.energy.or.kr | 국내 RE100 조달 수단 및 정보 접근 현황 |
| [^6] | K-ETS 3기 계획 수립 방안 | 환경부 | 2025 | https://www.me.go.kr | 무상할당 축소·탄소비용 증가 예고 |
| [^7] | 지속가능경영보고서 2025 | 삼성전자 | 2025 | https://www.samsung.com/sec/sustainability | RE100 달성 투자 규모 수조원대 |
| [^9] | 국가 온실가스 인벤토리 보고서(2024년판) | 온실가스종합정보센터(GIR) | 2024 | https://www.gir.go.kr | 발전원별 배출계수(유연탄 991, LNG 493, 원자력 12, 태양광 41, 풍력 11 gCO₂/kWh) |
| [^11] | 2024년 전력시장통계 | 전력거래소(KPX) | 2024 | https://www.kpx.or.kr | 국내 전력 탄소집약도 산출 기반 데이터 |
| [^12] | The A List: Companies Leading on Environmental Transparency | CDP | 2024 | https://www.cdp.net/en/articles/investor/the-a-list | CDP 미제출 기업에 대한 기관투자자 평가 영향 |

---

## F. 추정값 별도 목록 (검증 대기)

> 아래 항목은 제안서 본문에 `[추정]`으로 표기된 수치다. 정식 출처가 확보되면 위 표로 이관하고 `[추정]`을 제거한다.

| 추정값 | 근거/가정 | 검증 방법 |
|:---|:---|:---|
| 국내 ESG 컨설팅·탄소공시 시장 연 1,000억~5,000억원 | MarketsandMarkets 글로벌 CAGR 28% + 국내 GDP 비중 환산 | 국내 전문기관(에너지경제연구원 등) 보고서 확인 필요 |
| 담당자 월 20~40시간 CDP 작성 공수 | B2B SaaS 업계 벤치마크(Carbon6 등 유사 서비스 고객 인터뷰 인용) | 국내 대기업 ESG 담당자 인터뷰 필요 |
| CAC 500만원, LTV 1.08억원, LTV/CAC 21.6배 | B2B SaaS 업계 평균 + 직접 영업 비용 모델링 | 실제 파일럿 결과로 교체 필요 |
| 탄소집약도 차이 15분 기준 최대 3배 | 전력거래소 과거 발전믹스 데이터 패턴 분석[추정] | 실제 API 데이터 6개월 수집 후 검증 |
| 시간대 선택으로 탄소배출 30~60% 감축 | Tranberg et al.(2019) 유럽 결과의 한국 적용 [추정] | 국내 발전믹스 실제 데이터로 재산출 필요 |
| SAM 대기업 협력사 압력받는 중견기업 약 200개사 | 삼성·SK·LG 공급망 공개 데이터 추정 | 공급망 실사(ESG Due Diligence) 대상 기업 공시 확인 |

---

## G. 향후 추가 조사 계획

| 우선순위 | 조사 대상 | 목적 | 출처 후보 |
|:---:|:---|:---|:---|
| 1 | 국내 RE100 기업별 연도별 조달률 추이 (44개사 개별) | 타깃 고객 pain point 정량화 | CDP 한국 공시 데이터, 기업별 지속가능경영보고서 |
| 2 | 전력거래소 발전원별 발전량 API 실제 데이터 샘플 | 탄소집약도 산출 알고리즘 검증 | data.go.kr API 직접 호출 |
| 3 | 국내 제3자 PPA 계약 단가·지역별 분포 | 조달 시뮬레이터 가격 모델 | 에너지공단 PPA 거래 통계, RE100 계약 공시 |
| 4 | K-RE100 제도 이행 현황 | 국내 제도 연계 기능 설계 | 산업통상자원부 K-RE100 운영 현황 보고서 |
| 5 | electricityMap 국내 데이터 커버리지 현황 | 직접 경쟁 분석 | electricityMap.org API 테스트 |
| 6 | CDP/GRI 보고서 작성 비용 국내 실태조사 | CAC·가치 제안 수치화 | 국내 ESG 컨설팅사 공개 단가표, 실사례 인터뷰 |
