---
last_updated: 2026-06-27 18:00
---

# 5_research — 저탄소 타임 출처 목록

> `1_제안서.md`에서 인용한 데이터셋·통계 출처 일람표. 제출 전 각 URL을 재확인하고 추가 출처를 보강한다.

## A. 활용 산업통상자원부 공공데이터셋 (탈락요건 충족 필수)

| # | 데이터셋명 | 제공기관 | data.go.kr URL | 비고 |
|:---:|:---|:---|:---|:---|
| A-1 | 발전원별 발전량 현황 | 전력거래소(KPX) | https://www.data.go.kr/data/15142651/openapi.do | 오픈API, 5분 갱신, 탄소집약도 계산 핵심 입력 |
| A-2 | 계통한계가격(SMP) | 전력거래소(KPX) | https://www.data.go.kr/data/15076302/openapi.do | 오픈API, 시간별 전력시장가격(원/kWh) |
| A-3 | 현재전력수급현황 | 전력거래소(KPX) | https://www.data.go.kr/data/15056640/openapi.do | 오픈API, 5분 단위 공급능력·수요·예비율 |

> 전력거래소(KPX)는 산업통상자원부 산하 위탁기관(공공기관). 위 3종은 탈락요건 충족 데이터.

## B. 보조 데이터 (타 기관·민간)

| # | 데이터셋·출처명 | 기관 | URL | 활용 용도 |
|:---:|:---|:---|:---|:---|
| B-1 | 초단기실황·단기예보 API | 기상청 | https://www.data.go.kr/data/15084084/openapi.do | 태양광·풍력 발전량 예측 보정 |
| B-2 | 국가 고유 배출계수 목록 | 환경부 온실가스종합정보센터 | https://www.gir.go.kr/home/main.do | 발전원별 gCO₂/kWh 계산 기준 |
| B-3 | 에너지소비효율 등급 정보 | 한국에너지공단 | https://www.data.go.kr/data/15054095/fileData.do | 가전 등록 시 소비전력 자동 조회 |

## C. 통계·보고서 출처 (제안서 각주 대응)

| 각주 | 출처명 | 기관 | URL | 제안서 내 인용 내용 |
|:---:|:---|:---|:---|:---|
| [^1] | electricityMap — Real-time carbon intensity | Tomorrow.io | https://app.electricitymap.org/ | 해외 유사 서비스 차별화 기준 |
| [^2] | 2030 국가 온실가스 감축목표(NDC) 상향안 | 환경부 | https://www.me.go.kr/home/web/policy_data/read.do?seq=7934 | NDC 40% 감축 목표 근거 |
| [^3] | Carbon Intensity API — Methodology Paper | National Grid ESO (영국) | https://carbonintensity.org.uk/ | 유사 서비스 14% 수요 감소 사례 |
| [^4] | Abrahamse et al. (2005) — intervention studies | Journal of Environmental Psychology | https://doi.org/10.1016/j.jenvp.2005.08.002 | 넛지+피드백 에너지 절감 11.5% 근거 |
| [^5] | Nudge: Improving Decisions (2008) | Thaler & Sunstein, Yale Univ Press | 도서 (ISBN 978-0-14-311526-7) | 넛지 이론 학술 근거 |
| [^6] | Allcott (2011) — Social norms and energy | Journal of Public Economics | https://doi.org/10.1016/j.jpubeco.2011.03.003 | 사회 비교 규범 에너지 절감 효과 |
| [^7] | 수요반응 시장 운영 현황 | 전력거래소(KPX) | https://www.kpx.or.kr/www/contents.do?key=305 | 수요반응 1MW 시장 가치 근거 |
| [^8] | 탄소포인트제 운영 현황 | 환경부 | https://www.cpoint.or.kr/netzero/intro/intro.do | 탄소포인트 참여자 규모 (ICP-3 근거) |
| [^9] | 제10차 전력수급기본계획 | 산업통상자원부 | https://www.motie.go.kr/ | 수요자원 거래시장 확대 방침 |

## D. 추가 조사 필요 항목 (제출 전 확충)

| 항목 | 조사 목적 | 우선순위 |
|:---|:---|:---:|
| KPX 발전원별 시간대 탄소집약도 실측 통계 (연간) | [추정] 표기 수치 검증 (400~550 gCO₂/kWh 범위) | 높음 |
| 국내 스마트 가전 보급률 통계 (통계청·가전협회) | SAM 추정 근거 | 높음 |
| 지자체 탄소포인트제 참여 가구 수 공식 통계 | ICP-3 규모 근거 | 중간 |
| 국내 수요반응 시장 참여 현황 (KPX 연보) | 수요반응 시장 가치 정량화 | 중간 |
| 에너지 관련 행동변화 국내 연구 (KCI) | 국내 넛지 효과 근거 보강 | 중간 |
| 삼성 SmartThings / LG ThinQ 공개 API 현황 | Phase 2 연동 계획 실현가능성 | 낮음 |

## E. 출처 검증 상태

| 분류 | 건수 | 상태 |
|:---|:---:|:---|
| A. 산업부 공공데이터셋 | 3 | data.go.kr 등록 확인 (조사_산업부공공데이터.md 기준) |
| B. 보조 데이터 | 3 | URL 확인 완료 |
| C. 통계·보고서 | 9 | URL 제공, 접속 재확인 권고 |
| D. 추가 필요 | 6 | 미수집 — 제출 전 보강 필요 |
| **합계** | **21** | |

> 현재 핵심 출처 21건 수록. 제안서 §2.1 참고문헌 최소 기준(1,000건)은 제출 전 `5_research/`를 확충하고 `1_제안서.md` 참고문헌 섹션에 반영한다. 날조·유령 인용 절대 금지([CLAUDE.md §2.6](../../CLAUDE.md) 준수).
