last_updated: 2026-06-27 15:00

# 5_research — 데이터셋·출처 목록 (R&D 내비)

> 본 디렉터리는 `/12-R&D-과제공고-매칭/biz/1_제안서.md` 가 인용하는 모든 데이터셋·문헌의 출처 목록이다.
> 각 항목은 실재 확인된 정보만 등재한다. 미확인 항목은 `[확인필요]`로 명시.

---

## A. 핵심 산업부 공공데이터 (탈락요건 충족, 필수)

**표 A.** 활용 산업통상자원부 공공데이터셋

| # | 데이터셋명 | 제공기관 | 소관 부처 | 데이터셋 번호 | data.go.kr URL | 형식 | 갱신 주기 | 활용 목적 |
|:---:|:---|:---|:---|:---:|:---|:---:|:---:|:---|
| 1 | 산업기술 R&D 과제현황 | 산업기술기획평가원(KEIT) | 산업통상자원부 | 15018033 | https://www.data.go.kr/data/15018033/fileData.do | 파일(CSV) | 연간 | 선행과제 벡터 인덱스, 유사 레퍼런스 추출 |
| 2 | 산업기술기획평가원 사업공고 현황 | 산업기술기획평가원(KEIT) | 산업통상자원부 | 15130496 | https://www.data.go.kr/data/15130496/fileData.do | 파일(CSV) | 수시 | 매일 신규 공고 수집, 기업 매칭 엔진 입력 |
| 3 | 산업기술통계 | 산업기술진흥원(KIAT) | 산업통상자원부 | 15088711 | https://www.data.go.kr/data/15088711/fileData.do | 파일 | 연간 | 기업 프로필 업종·기술분야 분류 체계 참조 |

> 위 3종은 모두 산업통상자원부 산하 기관(KEIT·KIAT) 공개 데이터이며, 공모전 탈락요건(산업부·산하기관 데이터 활용)을 충족한다.

---

## B. 보조 데이터·참고 자료

**표 B.** 타 기관·민간 보조 데이터

| # | 자료명 | 기관 | URL | 활용 목적 |
|:---:|:---|:---|:---|:---|
| B1 | 범부처통합연구지원시스템(IRIS) 사업공고 | 과학기술정보통신부 등 | https://www.iris.go.kr | 보조 채널 공고 수집 |
| B2 | 국가과학기술표준분류체계(NTIS) | 한국과학기술정보연구원(KISTI) | https://www.ntis.go.kr | 기술 키워드 표준화 |
| B3 | 표준산업분류(KSIC) | 통계청 | https://kssc.kostat.go.kr | 기업 업종 분류 |
| B4 | 중소기업 기술로드맵 | 중소벤처기업부 | https://smtech.go.kr | 기업 기술 성숙도 맵핑 참조 |
| B5 | 중소기업 R&D 실태조사 | 중소벤처기업부 / KIAT | https://www.mss.go.kr | 시장 규모·TAM 추정 참고 |

---

## C. 기술 문헌 (AI·임베딩)

**표 C.** AI 기술 레퍼런스

| # | 문헌명 | 저자·기관 | 연도 | URL | 활용 |
|:---:|:---|:---|:---:|:---|:---|
| C1 | Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks | Reimers & Gurevych | 2019 | https://arxiv.org/abs/1908.10084 | 의미 유사도 매칭 기반 기술 |
| C2 | Billion-scale similarity search with GPUs (FAISS) | Johnson et al. (Meta AI) | 2019 | https://arxiv.org/abs/1702.08734 | 벡터 인덱스 기반 기술 |
| C3 | KLUE: Korean Language Understanding Evaluation | KLUE Team | 2021 | https://arxiv.org/abs/2105.09680 | klue/roberta-base 모델 기반 |
| C4 | Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks (RAG) | Lewis et al. (Meta AI) | 2020 | https://arxiv.org/abs/2005.11401 | 선행과제 레퍼런스 RAG 파이프라인 기반 |

---

## D. 공모전·정책 자료

**표 D.** 공모전·산업부 정책 참고 자료

| # | 자료명 | 기관 | URL | 활용 |
|:---:|:---|:---|:---|:---|
| D1 | "제14회 산업통상자원부 공공데이터 활용 아이디어 공모전 개최" | 전자신문 | https://www.etnews.com/20260330000032 | 공모전 개요·일정·부문 |
| D2 | "공공데이터로 창업·혁신 이끈다…산업부 아이디어 공모전" | 지이코노미 | https://www.geconomy.co.kr/mobile/article.html?no=318328 | 상금·지원 자격 |
| D3 | 제13회 공모전 결과 보도자료 | 정책브리핑 | https://admin2.korea.kr/briefing/pressReleaseView.do?newsId=156683863 | 13회 수상작 차별화 기준선 |
| D4 | 제13회 대상 수상 기사 | 아주경제 | https://www.ajunews.com/view/20250911094214407 | 수상작 상세 확인 |

---

## E. 확인 필요 항목

- [ ] KEIT 15130496 (사업공고 현황) 데이터셋의 정확한 갱신 주기 및 공공누리 라이선스 유형
- [ ] KEIT 15018033 (R&D 과제현황) 파일 컬럼 구조 (과제명·기술분류·주관기관 등 필드 확인)
- [ ] KIAT 15088711 (산업기술통계) 최신 데이터 연도 확인
- [ ] 각 데이터셋 상업적 활용 가능 여부 (공공누리 제1유형 여부)

---

## F. 조사 한계 및 추정값 고지

- 시장 규모(TAM·SAM·SOM), CAC, LTV, 매출 시나리오는 모두 `[추정]`으로 표기된 추정치다.
- 중소기업 R&D 공고 탐색 시간(월 8~20시간), 전담 인력 보유율 등은 제안서 작성 시점 공식 통계 출처를 확보하지 못하여 현장 인터뷰 참고·추정값을 사용하였다.
- 추가 출처는 제출 전 `5_research/` 내 세부 파일로 보강할 예정이다.
