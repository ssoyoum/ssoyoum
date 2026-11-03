<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:0f766e&height=180&section=header&text=%EB%B0%95%EC%86%8C%EC%98%81%20%7C%20AI%20%26%20Spatial%20Data%20Developer&fontSize=30&fontColor=ffffff&fontAlignY=38&desc=%EC%88%98%EC%9E%90%EC%9B%90%C2%B7%EA%B3%B5%EA%B0%84%EC%A0%95%EB%B3%B4%20%EC%8B%A4%EB%AC%B4%20%E2%86%92%20GIS%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%C2%B7%20AI%20Agent&descSize=16&descAlignY=58" width="100%" alt="박소영 | AI & Spatial Data Developer" />
</p>

<p align="center">
  공간정보·수자원 실무 경험을 바탕으로<br>
  <b>GIS 기반 서비스</b>와 <b>AI Agent</b>를 개발합니다.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/🏆_국토교통부_공간정보_활용_사례_분야-진흥원장상-f59e0b?style=flat-square" alt="진흥원장상" />
  <img src="https://img.shields.io/badge/🌊_2026_AI·디지털_사회문제_해결_챌린지-서류_합격-0ea5e9?style=flat-square" alt="서류 합격" />
  <img src="https://img.shields.io/badge/💬_2026_모두의_AI_실험실-선정-8b5cf6?style=flat-square" alt="모두의 AI 실험실 선정" />
</p>

---

## 🙋‍♀️ About Me

| | |
|---|---|
| 🎓 **전공** | 건설시스템공학 + 환경공학 |
| 🌊 **실무** | 수자원·공간정보 실무 약 4년 (홍수위험지도·하천 설계 자료) |
| 🗺️ **GIS** | 기관·좌표계가 다른 공공데이터를 건물·시설 단위로 묶는 데이터 처리와 WebGIS |
| 🤖 **AI** | FastAPI 기반 AI 서비스 · LLM이 고르고 서버가 확인하는 Agent 도구 실행 |

```mermaid
flowchart LR
  A["🗂️ 공공데이터<br/>수위 · 강우 · 건축물 · 침수지도"] --> B["🧹 정제 · 좌표계 통일<br/>Python · GeoPandas"]
  B --> C["⚙️ 판정 규칙 · API<br/>FastAPI"]
  C --> D["🤖 Agent 도구 실행<br/>Gemini · 서버 검증"]
  C --> E["🗺️ 지도 화면<br/>React · Leaflet · MapLibre"]
  D --> E
  F["✅ 고정 평가 · 테스트 · CI"] -.-> C
  F -.-> D
```

---

## 🚀 Featured Projects

### 1. 🏙️ 먼저 가야 할 집

<a href="https://basement-flood.duckdns.org"><img src="https://raw.githubusercontent.com/ssoyoum/Basement-Flood-Vulnerability/main/docs/assets/readme/hero.png" alt="먼저 가야 할 집 — 건물 단위 현장조사 우선순위 지도" width="100%" /></a>

**GIS 기반 주거 정보 서비스** — 서울 지하층 건물의 침수 정보를 한 동 단위로 조회하고, 먼저 확인할 집을 고릅니다.

| 무엇을 했나 | 숫자 |
|---|---|
| 기관·좌표계가 다른 **공공데이터 6종 통합** | 📊 지하층 **377,157동** 등급화 |
| **좌표계·데이터 단위 표준화** 후 건물 한 동 단위로 결합 | 🏠 먼저 확인할 집 **489동** |
| 공간정보와 **건축물대장 연계**, 침수지도가 없는 구는 "위험 없음"으로 두지 않는 대체 규칙 | 🗺️ 대체 규칙 적용 **11개 구** |

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/GeoPandas-139C5A?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=leaflet&logoColor=white" />
</p>

[📂 Repository](https://github.com/ssoyoum/Basement-Flood-Vulnerability) | [🌐 Demo](https://basement-flood.duckdns.org) | [🧩 Architecture](https://github.com/ssoyoum/Basement-Flood-Vulnerability/blob/main/docs/assets/system-architecture.svg)

---

### 2. 🌊 만약에 침수

<table>
  <tr>
    <td width="50%" align="center"><img src="https://raw.githubusercontent.com/ssoyoum/Flood-Disaster-Digital-Twin/main/docs/screenshots/ops-watch.png" alt="전국 감시 화면" width="100%" /><br><sub>전국 하천 접점 시설 감시</sub></td>
    <td width="50%" align="center"><img src="https://raw.githubusercontent.com/ssoyoum/Flood-Disaster-Digital-Twin/main/docs/screenshots/ops-agent.png" alt="Agent 대화 화면" width="100%" /><br><sub>도구를 골라 근거로 답하는 Agent</sub></td>
  </tr>
</table>

**AI 기반 침수 대응 서비스** — 수위·강우·특보를 지하차도·하천변 시설의 위험 단계로 바꿔 «어디를 먼저 막을지» 고르게 돕습니다.

```mermaid
flowchart LR
  Q["👤 질문"] --> L["🤖 Gemini<br/>도구 선택"]
  L --> V{"🛡️ 서버 확인<br/>도구명 · 입력값"}
  V -- 통과 --> T["🔧 읽기 전용 도구 실행"]
  V -- 거절 --> N["📋 필요한 자료와 한계 안내"]
  T --> R["💬 근거와 함께 답변"]
```

- **FastAPI 기반 Agent 도구 구현** — 등록된 읽기 전용 도구만 실행
- **Gemini API 연동** — SDK 없이 직접 호출, 답의 숫자가 도구 결과와 다르면 서버가 바로잡음
- **도구 실행 검증 및 테스트** — 43문항 고정 평가 **43/43**, 근거 없는 주장 **0건**, 토큰 **−21%**
- 600 MB 컨테이너의 메모리 부족 원인을 찾아 **663 → 506 MiB**

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Gemini_API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
</p>

[📂 Repository](https://github.com/ssoyoum/Flood-Disaster-Digital-Twin) | [🌐 Demo](https://floodops.duckdns.org) | [🧩 Architecture](https://github.com/ssoyoum/Flood-Disaster-Digital-Twin/blob/main/docs/ARCHITECTURE.md)

---

### 3. 🛰️ FloodOps / HAND Osong

<a href="https://floodops.duckdns.org"><img src="https://raw.githubusercontent.com/ssoyoum/Flood-Disaster-Digital-Twin/main/docs/screenshots/hero.gif" alt="사건 단계가 진행되며 침수 추정 셀이 번지는 사례 재생" width="100%" /></a>

**수자원·침수 분석 서비스** — 2023 오송 지하차도 등 과거 홍수 사례를 관측 자료로 단계별로 다시 재생하고, 같은 판정 규칙을 실제 통제 시각에 채점합니다. (‘만약에 침수’ 레포의 사례 재생 기능)

- **공간정보 및 수자원 도메인 적용** — 지형(HAND) 기반 침수 범위 근사, 계획홍수위·상승 속도로 통제 검토 시점 계산
- **API 기반 데이터 처리** — 홍수통제소·기상청 관측 자료로 오송·서울·포항·안동 **4개 사례** 재구성
- **서비스 기능 구현** — 궁평2 지하차도 규칙 백테스트에서 유입 **157분 전** 첫 검토, 늦었던 사례도 표에 그대로 남김

> HAND 침수 범위는 임시 근사이며 공식 침수범위나 수리해석 결과가 아닙니다. 백테스트는 실시간 경보 성능이 아닙니다.

[📂 Repository](https://github.com/ssoyoum/Flood-Disaster-Digital-Twin) | [🌐 Demo](https://floodops.duckdns.org) | [🧩 Architecture](https://github.com/ssoyoum/Flood-Disaster-Digital-Twin/blob/main/docs/CASE_REPLAY.md)

---

### ➕ More

| Project | 한 줄 |
|---|---|
| 🔥 [철든신입](https://github.com/steel-rookie/ST-ROOKIE) (팀) | 철강 신입사원 학습 서비스. 담당: JWT 로그인 API, 출처 재확인 학습 튜터, Langfuse trace |
| 🗺️ [의성 유휴자원 정책검토](https://github.com/ssoyoum/Uiseong-Resource-Model) | 전통수리시설 '못' 427개 × 생활권 인구, 현장검토 양식 116개 |
| 💬 [통해](https://github.com/ssoyoum/tonghae) (팀) | 이주노동자 생활 대화 도우미. 앱스토어 리뷰 3,889건 분석으로 기획 · [Demo](https://ssoyoum.github.io/tonghae/) |

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,react,ts,postgres&theme=light" alt="Python, FastAPI, React, TypeScript, PostgreSQL" /><br>
  <img src="https://skillicons.dev/icons?i=docker,githubactions,aws,git&theme=light" alt="Docker, GitHub Actions, AWS, Git" /><br>
  <img src="https://img.shields.io/badge/QGIS-589632?style=for-the-badge&logo=qgis&logoColor=white" alt="QGIS" />
  <img src="https://img.shields.io/badge/LLM_·_RAG-111827?style=for-the-badge&logo=googlegemini&logoColor=white" alt="LLM · RAG" />
</p>

| 분야 | 기술 |
|---|---|
| **AI** | LLM · RAG · Gemini API · Agent 도구 실행 · 고정 평가 |
| **Backend** | Python · FastAPI · PostgreSQL · SQLite |
| **Frontend** | React · TypeScript · Leaflet · MapLibre |
| **Spatial** | QGIS · GeoPandas · 좌표계 변환 · HAND |
| **DevOps** | Docker · GitHub Actions · AWS EC2 |

---

<p align="center">
  <a href="https://www.gitanimals.org/en-US?utm_medium=image&utm_source=ssoyoum&utm_content=farm">
    <img src="https://render.gitanimals.org/farms/ssoyoum" width="600" height="300" alt="GitAnimals farm" />
  </a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f766e,100:0ea5e9&height=100&section=footer" width="100%" alt="" />
</p>
