last_updated: 2026-06-27 14:00

# 5_research — 데이터셋·통계 출처 목록

> 본 아이디어(바이어 브릿지 — 실거래 전환형 AI 바이어 매칭) 제안서에서 인용한 데이터셋·통계의 출처 표. 제안서 각주(`[^N]`)와 1:1 대응. 정직성 원칙: 실재 확인된 출처만 기재, 미확인 항목은 [확인필요] 표기.

---

## 1. 산업통상자원부 산하기관 공공데이터 (탈락요건 핵심)

**표 1.** 활용 산업부 공공데이터셋

| 순번 | 데이터셋명 | 제공 기관 | 등록번호 | data.go.kr URL | 형식 | 확인 여부 |
|:---:|:---|:---|:---:|:---|:---:|:---:|
| 1 | 국가정보 | KOTRA (대한무역투자진흥공사) | 15034830 | https://www.data.go.kr/data/15034830/openapi.do | API | ✅ |
| 2 | 해외시장뉴스 | KOTRA | 15034831 | https://www.data.go.kr/data/15034831/openapi.do | API | ✅ |
| 3 | 한국무역현황 상세통계 | KOTRA | 15140428 | https://www.data.go.kr/data/15140428/fileData.do | 파일(CSV) | ✅ |
| 4 | 국가목록(264개국) | 한국무역보험공사(K-SURE) | 15144256 | https://www.data.go.kr/data/15144256/openapi.do | API | ✅ |

> 출처: `../../../planning/조사_산업부공공데이터.md §2. 무역/수출` 섹션에서 확인.

---

## 2. 통계·보고서 출처 (제안서 각주 대응)

**표 2.** 인용 통계 및 보고서

| 각주 | 명칭 | 기관 | 발행 | 핵심 수치 | URL / 출처 |
|:---:|:---|:---|:---:|:---|:---|
| [^1] | 중소기업 수출 현황 — 수출 중소기업 95,905개사 | 관세청·중소벤처기업부 | 2023 | 95,905개사 | 출처: `조사_문제landscape.md §4 [T8]` (원문 URL 추가 확인 필요) |
| [^2] | 수출 중소기업 실태조사 — 1년 생존율 49.2% | KOTRA | 2023~2024 | 수출 1년 생존율 49.2% | 출처: `조사_문제landscape.md §4 [T8]` |
| [^3] | 수출 애로 조사 — 바이어 발굴 22.5% 1위 | 중소기업중앙회·KOTRA | 2023~2024 | 바이어 발굴 22.5% | 출처: `조사_문제landscape.md §4 [T5]` |
| [^4] | buyKOREA 전환율 약 0.5%, 트라이빅 127건 | 언론 보도·업계 자료 | 2023~2024 | 전환율 0.5%, 성사 127건 | 출처: `조사_문제landscape.md §4` (원문 URL 추가 확인 필요) |
| [^5] | 수출/GDP 비율 | 한국은행·산업통상자원부 | 2025 | 43.9% [확인필요] | 한국은행 경제통계시스템(ECOS) — https://ecos.bok.or.kr (직접 확인 필요) |
| [^6] | Blue Ocean Strategy | Kim, W.C. & Mauborgne, R. | 2004/2015 | ERRC 프레임워크 | Harvard Business Review Press |
| [^7] | The Lean Startup | Ries, E. | 2011 | Build-Measure-Learn | Crown Business |

---

## 3. 추가 조사 필요 항목 (미확인·[추정] 수치)

**표 3.** 향후 검증 필요 수치

| 수치 | 현재 상태 | 검증 방법 |
|:---|:---:|:---|
| 외부 컨설팅 비용 연 1,500만 원/사 | [추정] | KOTRA 수출 지원 비용 조사, 관세사·무역컨설팅 업체 견적 조사 |
| 담당자 바이어 탐색 공수 주 5~10시간 | [추정] | 수출 중소기업 인터뷰 또는 설문 필요 |
| 전환율 개선 목표 5~10% | [추정] | 시범 기업 30개사 파일럿 결과로 검증 |
| CAC 약 50만 원/사 | [추정] | 초기 마케팅 집행 후 실측 |
| LTV 약 250만 원/사 | [추정] | 1년차 코호트 이탈률 관찰 후 갱신 |
| 수출 1년 생존율 → 55% 개선 | [추정] | 3년 후 코호트 추적 조사 |
| 수출/GDP 43.9% (2025) | [확인필요] | 한국은행 ECOS, 산업통상자원부 수출입 동향 |
| FTA 활용률 중소 61.5% vs 대기업 85.1% | `조사_문제landscape.md §4 [T11]` | 산업통상자원부 FTA 활용 실태조사 원문 URL 확인 |
| 해외인증 비용 연 약 2.3조 | `조사_문제landscape.md §4 [T12]` | 기술표준원·한국인증원 등 공식 보고서 확인 |

---

## 4. 참고 기술 자료

**표 4.** AI·기술 참고 자료

| 명칭 | 유형 | URL / 출처 |
|:---|:---:|:---|
| Sentence-Transformers (paraphrase-multilingual-mpnet-base-v2) | 오픈소스 모델 | https://huggingface.co/sentence-transformers/paraphrase-multilingual-mpnet-base-v2 |
| FAISS — Facebook AI Similarity Search | 오픈소스 라이브러리 | https://github.com/facebookresearch/faiss |
| XGBoost 공식 문서 | 오픈소스 라이브러리 | https://xgboost.readthedocs.io |
| SHAP (SHapley Additive exPlanations) | XAI 라이브러리 | https://github.com/shap/shap |
| LangChain (RAG 파이프라인) | 오픈소스 프레임워크 | https://python.langchain.com |

---

## 5. 경쟁사·시장 참고

**표 5.** 경쟁 서비스 참고 자료

| 서비스명 | 운영 기관 | URL | 조사 내용 |
|:---|:---|:---|:---|
| buyKOREA | KOTRA | https://www.buykorea.or.kr | 노출형 카탈로그, 전환율 약 0.5% |
| TradeKorea | KOTRA 연계 | https://www.tradekorea.com | 카테고리 디렉토리 방식 |
| KOTRA Gep | KOTRA | https://gep.kotra.or.kr | 바이어 DB 수동 검색 |
| KOTRA 트라이빅(Tri-Vig) | KOTRA | — | 2023 매칭 성사 127건 |
| FTA-PASS | 관세청·무역협회 | https://ftapass.or.kr | 관세율 조회, 능동 추천 약함 |
| 트레이드내비(TradeNAVI) | 무역협회 | https://www.tradenavi.or.kr | 품목별 수출 조회 중심 |

---

> 출처 기반 조사 심화 방향: `조사_문제landscape.md §4` 무역·수출 영역 각 번호([T5][T8][T11][T12])에 대한 원문 URL 추적 조사, KOTRA 공식 보고서 다운로드 후 수치 재확인 권장.
