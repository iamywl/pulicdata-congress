last_updated: 2026-06-27 18:00

# 5_research — 데이터셋·통계 출처 목록

> 본 파일은 `/biz/1_제안서.md`가 인용하는 모든 데이터셋·통계·문헌의 단일 출처 목록이다.
> 추가 조사 시 이 파일에 행을 추가하고 제안서 각주와 1:1 대응시킨다.

---

## 1. 산업부 공공데이터셋 (탈락요건 충족 필수 항목)

| # | 데이터셋명 | 기관 | data.go.kr URL | 형식 | 갱신 | 활용 |
|:---:|:---|:---|:---|:---:|:---:|:---|
| D-1 | 해외시장뉴스 | KOTRA (대한무역투자진흥공사) | https://www.data.go.kr/data/15034831/openapi.do | API | 일 | RAG Vector DB 원천: 인증·규제 정보 |
| D-2 | 국가정보 | KOTRA | https://www.data.go.kr/data/15034830/openapi.do | API | 분기 | RAG 보조: 국가별 경제·무역 환경 |
| D-3 | 한국무역현황 상세통계 | KOTRA | https://www.data.go.kr/data/15140428/fileData.do | 파일 | 월 | 유망시장 추천 스코어링 엔진 원천 |
| D-4 | 국가목록 (264개국) | 무역보험공사 (K-SURE) | https://www.data.go.kr/data/15144256/openapi.do | API | 연 | 국가 리스크 등급 반영 |

---

## 2. 통계·정책 출처 (제안서 각주 대응)

| 각주 | 명칭 | 기관 | 핵심 수치 | URL |
|:---:|:---|:---|:---|:---|
| [^1] | 2023년 중소기업 수출 실태조사 | 중소벤처기업부 | 수출 중소기업 1년 내 중단율 50.8% | https://www.mss.go.kr |
| [^2] | 동일 | 중소벤처기업부 | 수출 애로 1위: 바이어 발굴·시장정보 부족 22.5% | 동상 |
| [^3] | FTA 활용 실태조사 | 산업통상자원부 | 중소기업 FTA 활용률 61.5%, 대기업 85.1% (23%p 격차) | https://www.motie.go.kr |
| [^4] | 중소기업 기업체 수 현황 | 통계청 KOSIS | 중소기업 약 60만 개사 | https://kosis.kr |
| [^5] | 수출입 동향 | 산업통상자원부 | 수출 중소기업 약 9.6만 개사 | https://www.motie.go.kr |

---

## 3. 경쟁·유사 서비스 참고

| 서비스명 | 운영 기관 | URL | 조사 내용 |
|:---|:---|:---|:---|
| FTA-PASS | 관세청 | https://www.ftapass.or.kr | FTA 세율 조회 기능, 유망국 추천 없음 확인 |
| 트레이드내비 | KOTRA | https://www.tradenavi.or.kr | 통계 기반 시장 조회, 인증 체크리스트 없음 확인 |
| buyKOREA | KOTRA | https://www.buykorea.org | 바이어 디렉토리 중심, 전략 추천 없음 |
| KOTRA 수출바우처 | KOTRA | https://www.exportvoucher.com | 컨설팅 바우처, 디지털 자동화 낮음 |

---

## 4. 기술·오픈소스 참고

| 항목 | 명칭·버전 | 라이선스 | URL |
|:---|:---|:---:|:---|
| 임베딩 모델 | bge-m3 (BAAI) | MIT | https://huggingface.co/BAAI/bge-m3 |
| 생성 LLM | EXAONE-3.5 (LG AI Research) | LG AI Research License | https://huggingface.co/LGAI-EXAONE/EXAONE-3.5-7.8B-Instruct |
| Vector DB | Chroma | Apache-2.0 | https://www.trychroma.com |
| 백엔드 | FastAPI | MIT | https://fastapi.tiangolo.com |
| 프론트엔드 | Next.js | MIT | https://nextjs.org |

---

## 5. 추가 조사 예정 항목 (초안 단계 미확인)

| 항목 | 필요 이유 | 우선순위 |
|:---|:---|:---:|
| 해외인증 비용 총액 (연 약 2.3조 원) | 제안서 본문 인용 — 출처 확인 필요 | 높음 |
| KOTRA 컨설팅 평균 대기 기간 | 시간 절감 가치 정량화 근거 | 중간 |
| FTA 미활용 원인 상세 (산업부 실태조사 원문) | [^3] 각주 원문 URL 확보 | 높음 |
| 수출바우처 선정 기업 수 (2026) | GTM 파일럿 대상 규모 산정 | 중간 |
| RAG 정확도 벤치마크 (무역 도메인) | 기술 구체성 보강 | 낮음 |

---

> **정직성 메모**: 위 항목 중 [추정] 표기된 수치(TAM/SAM/SOM, CAC, LTV, 전환율 등)는 현재 검증된 외부 출처가 없으며 제안서 내 [추정] 태그로 명시됐다. 정식 제출 전 추가 조사로 대체하거나 추정 근거를 보강한다.
