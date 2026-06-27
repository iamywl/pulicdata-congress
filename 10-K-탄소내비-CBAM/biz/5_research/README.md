---
last_updated: 2026-06-27 15:00
---

# 5_research — 출처·근거자료 목록 (K-탄소내비)

> 제안서 `1_제안서.md`가 인용하는 모든 공개 데이터셋·통계·문헌의 목록이다.
> 각 항목은 **명칭 · 기관 · URL · 제안서 내 활용 목적** 순으로 정리한다.
> `[확인필요]` 표시는 URL 또는 정확한 수치를 재검증해야 함을 의미한다.

---

## A. 산업통상자원부 산하기관 공공데이터셋 (탈락요건 충족)

> 아래 4종은 `1_제안서.md` §3-①에 명시된 핵심 공공데이터이며, 모두 data.go.kr에서 실재 확인된 데이터셋이다.

| # | 데이터셋명 | 제공기관 | 등록번호 | data.go.kr URL | 활용 목적 |
|:---:|:---|:---|:---:|:---|:---|
| DS1 | 한국산업단지공단 국가산단 입주업체 현황 | 한국산업단지공단 (KICOX) | 15085894 | https://www.data.go.kr/data/15085894/fileData.do | 대상 기업 식별·벤치마크·매칭 풀 구성 |
| DS2 | 한국전력 산업분류별 전력사용량 | 한국전력공사 (KEPCO) | 15101403 | https://www.data.go.kr/data/15101403/openapi.do | 업종별 전력 원단위 → 탄소집약도 추정 핵심 입력 |
| DS3 | 전력거래소 발전원별 발전량 현황 | 전력거래소 (KPX) | 15142651 | https://www.data.go.kr/data/15142651/openapi.do | 월별 전력 배출계수(kgCO₂/kWh) 산출 |
| DS4 | 산업기술진흥원 에너지 관련 성과 | 산업기술진흥원 (KIAT) | 15144954 | https://www.data.go.kr/data/15144954/fileData.do | 업종별 에너지절감 R&D 성과 → 매칭 추천 근거 |

---

## B. EU 규정·국제 기준 (RAG 인덱스 구성 원천)

| # | 명칭 | 기관 | URL | 활용 목적 |
|:---:|:---|:---|:---|:---|
| R1 | Regulation (EU) 2023/956 (CBAM Regulation) | European Commission / EUR-Lex | https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32023R0956 | CBAM 법적 근거·과태료 규정(Art. 22) |
| R2 | Implementing Regulation (EU) 2023/1773 | European Commission / EUR-Lex | https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32023R1773 | CBAM 보고서 항목·형식 상세 규정 |
| R3 | CBAM Declarant Portal 안내 자료 | European Commission CBAM Portal | https://cbam.ec.europa.eu | 보고서 제출 실무 가이드 |

---

## C. 국내 통계·보도자료 (문제 현황 근거)

| # | 명칭 | 기관 | URL | 제안서 활용 | 비고 |
|:---:|:---|:---|:---|:---|:---|
| I1 | CBAM 대응 중소기업 실태조사 | 중소기업중앙회 또는 산업통상자원부 | [확인필요] | 78.3% 미인지율·~1,400개사 추산 | [^1] — 원본 URL 재검증 필요 |
| I2 | 국가산업단지 분기별 동향 | 한국산업단지공단 (KICOX) | https://www.kicox.or.kr/publicData/publicDataList | 가동률 69.6%, -7.7%p | [^3] — 발행일·정확 URL 재검증 |
| I3 | 국가산단 입주업체 현황 (공공데이터포털 파일) | KICOX | https://www.data.go.kr/data/15085894/fileData.do | 입주업체 총 수(약 9만 개사) | DS1과 동일 데이터셋 |

---

## D. 보조 데이터·참고 자료

| # | 명칭 | 기관 | URL | 활용 목적 |
|:---:|:---|:---|:---|:---|
| S1 | KSIC 한국표준산업분류 코드체계 | 통계청 | https://kssc.kostat.go.kr | 업종 코드 매핑 |
| S2 | EU ETS 탄소가격 (EUA) 현황 | EU ETS 공개 포털 / ICE | https://www.theice.com/products/197684/EUA-Futures | CBAM 인증서 비용 추정 입력 |
| S3 | 온실가스종합정보센터 K-ETS 할당량 | 환경부 온실가스종합정보센터 | https://www.gir.go.kr | K-ETS 비교 대시보드 보조 |
| S4 | 조사_산업부공공데이터.md (내부 조사) | 워크스페이스 내부 | /Users/ywlee/pulicdata_congress/planning/조사_산업부공공데이터.md | 데이터셋 카탈로그 및 URL 초기 확인 |
| S5 | 조사_문제landscape.md (내부 조사) | 워크스페이스 내부 | /Users/ywlee/pulicdata_congress/planning/조사_문제landscape.md | 산업단지·CBAM 문제 현황 통계 초기 인용 |

---

## E. 향후 보강 필요 항목

> 제안서 초안 단계에서 [확인필요] 또는 [추정]으로 표기된 항목 중 외부 출처 확보가 필요한 것들이다.

| 항목 | 현재 상태 | 보강 방법 |
|:---|:---|:---|
| CBAM 미인지율 78.3% 원본 출처 | [확인필요] | 중기중앙회 보도자료 또는 산업부 CBAM 실태조사 원문 URL 확인 |
| CBAM 대상 중소업체 ~1,400개사 | [확인필요] | 산업부·KOTRA·무역협회 공개 추산치 원문 확인 |
| 민간 탄소 컨설팅 단가 300~800만 원 | [추정] | 국내 탄소 컨설팅사 공개 견적 또는 업계 보도 수집 |
| 시장 규모 (TAM·SAM·SOM) | [추정] | 국내 ESG·탄소 컨설팅 시장 리포트 (예: 한국기업지배구조원·딜로이트) 확보 |
| KICOX 분기 동향 정확 URL·발행일 | [확인필요] | KICOX 공식 통계 페이지 직접 확인 |
| EU CBAM 2030 품목 확대 계획 | [확인필요] | European Commission CBAM review 공식 문서 |

---

## 출처 수집 현황

| 구분 | 현재 수량 | 목표 |
|:---:|:---:|:---:|
| 산업부 공공데이터셋 | 4 | 4 (충족) |
| EU 규정·국제 기준 | 3 | — |
| 국내 통계·보도 | 3 | 확장 필요 |
| 보조·참고 | 5 | 확장 필요 |
| **합계 (고유 출처)** | **15** | **핵심 출처 확보 완료; 전체 확장은 개발 단계에서** |
