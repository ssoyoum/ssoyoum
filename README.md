# 박소영

### 수자원·공간정보 실무 → AI Agent · AI 서비스 개발

수자원 엔지니어링 실무 약 4년 동안 홍수위험지도·하천 설계 자료를 다뤘고,
지금은 그 도메인 데이터를 **사용자가 판단에 쓰는 AI 서비스**로 만드는 개발을 하고 있습니다.

일할 때 먼저 정하는 것은 **"자료가 답할 수 있는 범위"**입니다.
LLM이 고르는 일과 서버가 확인하는 일을 나누고, 고정 평가·테스트·CI로 결과를 확인합니다.

---

## Featured Projects

### 🌊 만약에 침수 — 홍수 통제 판단 지원 서비스 · [Repo](https://github.com/ssoyoum/Flood-Disaster-Digital-Twin) · [Demo](https://floodops.duckdns.org)

홍수통제소 수위·홍수특보와 기상청 강우·호우특보를 지하차도·하천변 출입구의 위험 단계로 바꿔 **어디를 먼저 막을지** 고르게 돕는 서비스입니다.

- **Agent:** LLM은 등록된 읽기 전용 도구만 고르고, 서버가 도구명·입력값을 확인한 뒤에만 실행합니다. 계산할 수 없는 질문에는 필요한 자료와 한계를 돌려줍니다.
- **평가:** 43문항 고정 평가로 한 번에 한 요소씩 고쳐 43/43, 근거 없는 주장 0건, 토큰 사용량 21% 감소
- **운영:** 600 MB 컨테이너에서 나던 메모리 부족 원인(같은 자료 반복 파싱)을 찾아 663 → 506 MiB로 줄임. GitHub Actions에서 테스트·Agent 평가·브라우저 회귀를 통과해야 Docker 이미지로 넘어가게 함
- **검증:** 같은 규칙을 과거 홍수의 실제 통제 시각에 채점하고, 늦었던 사례도 표에 그대로 남김
- 2026 AI·디지털 기반 사회문제 해결 챌린지 서류 합격

`Python` `FastAPI` `Gemini API` `React` `TypeScript` `Docker` `AWS EC2` `GitHub Actions`

### 🏙️ 먼저 가야 할 집 — 서울 지하층 침수 취약 건물 WebGIS · [Repo](https://github.com/ssoyoum/Basement-Flood-Vulnerability)

기관과 좌표계가 다른 공공데이터 6종을 건축물 한 동 단위로 묶어, 서울 지하층 건축물의 침수 정보를 조회하고 먼저 확인할 집을 고르는 WebGIS입니다.

- 서울 지하층 377,157동을 등급화해 예상 침수심 1.0 m 이상 주거용 지하층 489동을 먼저 확인할 집으로 선정
- 도시침수지도가 없는 11개 구를 "위험 없음"으로 두지 않고, 확인을 거쳐 서울시 침수예상도로 대체하는 규칙을 둠
- 분석 결과는 FastAPI·SQLite 읽기 전용 API로, 계정·현장기록은 PostgreSQL로 나눠 설계
- 국토교통부 주최 제8회 공간정보 활용·아이디어 경진대회 **공간정보 활용 사례 분야 진흥원장상**

`Python` `GeoPandas` `FastAPI` `SQLite` `PostgreSQL` `React` `Leaflet` `Docker`

### 🔥 철든신입 — 철강 신입사원 학습 서비스 (팀) · [Repo](https://github.com/steel-rookie/ST-ROOKIE)

포스코 K-뉴딜 아카데미 팀 프로젝트입니다. 제가 맡은 부분은 아래와 같습니다.

- Node.js·TypeScript 로그인 API(JWT)와, 기존 화면이 깨지지 않게 토큰·기존 방식을 함께 받는 호환 구조
- 학습 튜터가 검색한 자료의 출처 ID를 서버가 다시 확인하고, 보충학습 Agent에 도구 5개 연결
- 요청마다 검색·모델 판단·도구 실행·검증 단계를 남기는 trace를 OpenTelemetry로 Langfuse에 기록

`TypeScript` `Node.js` `JWT` `Gemini` `Ollama` `Langfuse` `OpenTelemetry`

### 그 밖의 프로젝트

| Project | 내용 |
|---|---|
| 🗺️ [의성 유휴자원 정책검토](https://github.com/ssoyoum/Uiseong-Resource-Model) | 의성군 전통수리시설 '못' 427개에 생활권 인구를 연결해 정책 검토 맥락과 현장검토 양식 116개 생성. 원자료 해시·핵심 수치를 파이프라인마다 검증 |
| 💬 [통해](https://github.com/ssoyoum/tonghae) | 이주노동자 생활 대화 도우미(팀). 4개국 앱스토어 리뷰 3,889건 분석으로 기획. 2026 모두의 AI 실험실 선정 · [Demo](https://ssoyoum.github.io/tonghae/) |
| 🧠 [Narrative Lab](https://github.com/ssoyoum/narrative-lab) | 검색용·생성용 Story DNA를 분리한 Narrative Engine |
| 🤖 [AI English Content Pipeline](https://github.com/ssoyoum/AI-english_content_pipeline) | AI 콘텐츠 생성 → JSON 검증 → TTS → 학습 UI로 잇는 파이프라인 |

---

## Tech

**AI / Agent**
LLM Tool Calling · RAG · Gemini API · OpenAI API · Ollama · Langfuse · Agent 평가

**Backend**
Python · FastAPI · Node.js · TypeScript · REST API · SQLite · PostgreSQL

**Frontend**
JavaScript · TypeScript · React · HTML · CSS

**Spatial / Data**
GIS · QGIS · GeoPandas · pandas · Leaflet · GeoJSON

**DevOps**
Git · GitHub Actions · Docker · AWS EC2

---

### Learning

- 포스코 K-뉴딜 아카데미 (2026.07 ~ 2026.11)
- 오르미 캠프 — Python·머신러닝 → LangChain 기반 RAG (2025.10 ~ 12)

<a href="https://www.gitanimals.org/en-US?utm_medium=image&utm_source=ssoyoum&utm_content=line">
  <img
    src="https://render.gitanimals.org/lines/ssoyoum"
    width="100"
    height="100"
  />
</a>

<a href="https://www.gitanimals.org/en-US?utm_medium=image&utm_source=ssoyoum&utm_content=farm">
<img
  src="https://render.gitanimals.org/farms/ssoyoum"
  width="600"
  height="300"
/>
</a>
