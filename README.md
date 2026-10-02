# 문영식 | Youngsik Moon

**고객의 문제를 발견하고, 사업 방향을 제안하며, 제품의 개발과 운영까지 책임지는 Product Engineer입니다.**

B2B 솔루션 개발, 엔터프라이즈 보안, 금융 IT 자동화, 인프라 운영과 직접 사업을 운영한 경험을 바탕으로 제품을 만듭니다. 고객을 만나 무엇이 필요한지 파악하고, 무엇을 왜 만들어야 하는지 판단해 기획부터 개발·배포·운영까지 연결합니다.

[직접 만든 제품 · BuildBrief](https://buildbrief.moon0sik.cloud) · [LinkedIn](https://www.linkedin.com/in/moonyoungsik95)

## 지금 하는 일

와이씨코퍼레이션에서 기업 업무 통합 B2B SaaS **SmartDash**를 주도적으로 기획하고 개발하고 있습니다.

- **사업 방향 제안:** Odoo 기반 사업을 준비하는 과정에서 예상되는 도입·운영 문제와 기존 자사 솔루션의 한계를 파악하고, 앞으로의 사업 방향에 맞는 새로운 자사 솔루션의 비즈니스 모델을 제안했습니다.
- **제품 구현과 운영:** 기능 기획, 시스템·UI/UX 설계, 프론트엔드·백엔드 개발, 데이터베이스, 인프라 구성, 배포와 운영까지 혼자 맡아 추진하고 있습니다.
- **고객 검증과 기술영업:** 고객을 직접 만나 데모와 컨설팅을 진행하고, 현장의 요구사항을 제품에 반영합니다. 직접 기술영업을 진행한 9개 고객사에서 도입 의향을 확인했으며, 정부지원사업에 선정되지 않은 경우에도 별도로 SmartDash 도입을 희망하는 고객이 생겼습니다.

## 일하는 방식

- **기술과 사업을 함께 봅니다.** 직접 사업을 운영하며 재고·매입·지출·근태·급여 관리를 시스템화했습니다. 기능의 구현 가능성과 함께 실제 업무, 비용, 운영에 미치는 영향을 생각합니다.
- **낯선 영역에도 직접 들어갑니다.** 작은 조직과 자원이 제한된 환경에서 사수 없이 필요한 기술을 익히고 프로젝트를 완수해 왔습니다. 필요한 일이면 익숙한 기술이나 역할 밖에서도 방법을 찾아 실행합니다.
- **AI를 활용하고 결과를 책임집니다.** 개발 전반에 AI를 적극 활용하되, 요구사항 분석과 기술적 의사결정, 구현 결과의 검증은 직접 수행합니다.
- **경험을 공유합니다.** LinkedIn에서 실무의 문제 해결 과정과 기술을 운영·보안·비용·사용자 경험의 관점으로 정리하고 있습니다.

## 개인 제품 · BuildBrief

**아이디어를 구체적인 기획으로 정리하고 AI 개발 도구에 전달하는 데 어려움을 겪는 사람들을 위해 직접 기획하고 개발한 제품입니다.**

AI로 개발할 수 있는 환경이 열려도, 만들고 싶은 것을 명확히 설명하고 기획하는 일은 여전히 어렵습니다. 아이디어가 있어도 바이브 코딩 도구에 의도를 제대로 전달하지 못하는 문제에 주목해 BuildBrief를 만들었습니다.

- **해결하려는 문제:** 머릿속 아이디어를 설명하고, 필요한 기능과 요구사항을 정리해 개발에 전달하는 과정의 어려움
- **제품 방향:** 아이디어를 구체화해 AI를 활용한 개발로 이어갈 수 있도록 돕는 서비스
- **현재 단계:** 상용화 전 프로토타입으로, 아이디어를 구체화하고 AI 개발 도구에 전달하는 핵심 흐름을 구현하는 데 집중했습니다.
- **향후 계획:** 사용자 피드백과 상용화 요구사항에 맞춰 기능과 기술 구조를 보완하며, 상용 솔루션으로 발전시킬 계획입니다.

[BuildBrief 사용해 보기](https://buildbrief.moon0sik.cloud/)

## 대표 실무 프로젝트

### SmartDash · 기업 업무 통합 B2B SaaS

그룹웨어, CRM, 견적·수주, 생산·재고, 인사·근태와 설비 데이터를 하나의 환경에서 관리하는 제품입니다.

**담당:** 비즈니스 모델 제안 → 고객 요구사항 정의 → 기획·설계 → 풀스택 개발 → 배포·운영 → 기술영업

**주요 기술:** Python, FastAPI, React, TypeScript, PostgreSQL, SQLAlchemy, Alembic, TanStack Query, Zustand, Valkey, MQTT, InfluxDB, AWS, GitHub Actions

| 해결한 문제 | 접근과 구현 |
| --- | --- |
| 기능 확장에 따라 흩어지는 업무 규칙 | 모듈러 모놀리식 구조 안에서 업무 경계를 나누고 생산·재고·결재의 공통 정책을 분리 |
| 결재선 조회의 반복 SQL | 관계 데이터 일괄 조회와 키 기반 매핑으로 변경. 격리 재현 테스트에서 SQL 실행 401회 → 5회, 응답 동일성 확인 |
| 동시 요청과 재시도로 인한 데이터 불일치 | 행 잠금, 잠금 순서 통일, 트랜잭션과 멱등 처리 적용 |
| 고객사·사용자별 데이터 접근 통제 | 회사·소유 관계·업무 권한 검사와 서버 세션 검증, 계정 전환 시 조회 캐시 분리 |
| 환경별 DB 변경과 배포 관리 | Alembic 리비전과 GitHub Actions를 연결해 마이그레이션·상태 확인 절차 구성 |
| 외부 메일 연동의 부분 실패 | SMTP 발송 성공과 보낸편지함 저장 실패를 구분해 중복 발송 방지 |

> SQL 수치는 결재선 100개·각 1단계·공통 결재자 조건의 SQLite 격리 재현 결과입니다. 운영 환경의 응답시간 개선율을 뜻하지 않습니다.

### SmartLine2 · 제조실행시스템(MES)

인수인계 문서 없이 소스 코드와 DB 접속 정보만 전달받은 환경에서 기존 구조와 업무 흐름을 분석하고, 웹 프론트엔드·백엔드의 기능 추가와 개선, 운영을 담당했습니다.

**주요 기술:** Spring Boot, React, PostgreSQL, MQTT, InfluxDB, AWS

### KPI 2.0 · 데이터 수집·전송 스케줄러

정부지원사업 OpenAPI 문서를 바탕으로 데이터 수집·전송 도구의 기획, 설계, UI, 개발과 운영을 맡았습니다.

**주요 기술:** Python, PySide6, PostgreSQL

### 그 밖의 실무 경험

- **MES 실행 장애 복구:** 고객사의 기존 MES 실행 불가 원인을 분석하고 복구 및 재발 방지를 위한 재빌드 수행
- **SmartLinePlus:** 자사 MES와 Odoo ERP 연동 및 커스텀 모듈 개발
- **협동로봇 커피머신:** 키오스크와 주문 관리 시스템 개발. 로봇 제어를 제외한 소프트웨어 담당
- **Autodesk Fusion 360 KPI 수집:** 데이터 수집·전송 유틸리티 기획, 개발과 운영

## 경력

| 기간 | 소속·활동 | 주요 경험 |
| --- | --- | --- |
| 2024.11–현재 | 와이씨코퍼레이션 · DX사업본부 수석연구원 / 매니저 | B2B SaaS·MES 기획과 개발, 인프라·운영, PM, 고객 컨설팅과 기술영업 |
| 2022년 시작 | 직접 사업 운영 | 재고·매입·지출·근태·급여 관리 시스템화 및 운영 프로세스 개선 후 사업 정리 |
| 2021.08–2023.02 | 센텍정보기술 · 기술본부 대리 / 매니저 | 금융·기업 고객의 배치 자동화 솔루션 JobMind 구축, POC, 운영과 기술지원 |
| 2019.04–2020.05 | 에스에스앤씨 · 기술본부 대리 / 매니저 | 엔드포인트·스마트팩토리 보안 솔루션 구축과 운영, POC, DB 마이그레이션 |
| 2017.10–2018.02 | 아이디스트 · 프리랜서 | SNS 마케팅 자동화 서비스 판매 페이지 개발, CS와 원격 기술지원 |

보안·금융 IT 현장에서 고객사와 협업하며 시스템의 안정성과 운영 요구를 익혔고, 직접 사업을 운영하면서 기술을 사용하는 사람의 입장도 경험했습니다. 지금은 이 경험들을 B2B 제품 개발에 연결하고 있습니다.

## 사용하는 기술

| 영역 | 기술 |
| --- | --- |
| Backend | Python, FastAPI, Java, Spring Boot, SQLAlchemy, Alembic |
| Frontend | React, TypeScript, TanStack Query, Zustand |
| Data & Messaging | PostgreSQL, MS SQL Server, Valkey / Redis, MQTT, InfluxDB |
| Infrastructure | Linux, AWS, Oracle Cloud Infrastructure, Docker, GitHub Actions |
| Desktop & Automation | PySide6, tkinter, Selenium |
| AI 프로젝트 경험 | LLM, NLP, 객체 탐지, STT / TTS, PyTorch |

## 공개 프로젝트와 기록

| 프로젝트 | 내용 |
| --- | --- |
| [Secu Book](https://github.com/YoungsikMoon/secu-book) | 커뮤니티와 함께 개선하는 웹 실무 보안 책 |
| [YouTube Downloader](https://github.com/YoungsikMoon/youtube-downloader-gui) | Excel 일괄 작업, 진행 상태와 실행 로그를 지원하는 Windows GUI 도구 |
| [InBest](https://github.com/YoungsikMoon/05.-InBest) | 금융·주식 도메인의 LLM 서비스 프로젝트 |
| [Object Detection](https://github.com/YoungsikMoon/04.-ObjectDetection) | 실종자 탐색과 낙상 감지 프로젝트 |
| [Find Imo](https://github.com/YoungsikMoon/03.-Find_Imo) | 면접 자동화 프로젝트 |
| [FORS](https://github.com/YoungsikMoon/02.-FORS) | STT·TTS 기반 장애인·고령자 취업 지원 프로젝트 |
| [Alpha911](https://github.com/YoungsikMoon/01.-alpha911) | NLP 기반 웹툰 인사이트 생성 프로젝트 |
| [Text Mining](https://github.com/YoungsikMoon/00.-Text-Mining) | 텍스트 분석 학습·집필 기록 |
| [전세버스 서비스 시연](https://www.youtube.com/watch?v=BDou4zE-RDQ) | Java 웹 개발 팀 프로젝트 |

<details>
<summary>교육·수상·자격</summary>

### 최근 교육

- Node.js + NestJS 교과서 기반 AI 서비스 개발 10주 챌린지 · 2026.06–2026.08
- MSA 아키텍처 풀스택 재직자 업스킬링 과정 · 2026.03–2026.07
- MES 구축, PLC·HMI·SCADA, 스마트 센서, 디지털 트윈 실무 교육 · 2025
- 머신러닝·딥러닝 개발 과정 · 2024.02–2024.08
- Kubernetes, Docker, Linux, Istio 관련 교육 · 2021–2022
- 웹 개발자를 위한 보안 프로그램 전문가 과정 · 2018.08–2019.04

### 수상

- 에이븐 기술 블로그 경진대회 1등 · 2025.02, 2회
- 디노랩스 MAI Agent·자동화 과정 2등 · 2024–2025, 2회
- 미래능력개발교육원 팀 프로젝트 최우수상 · 2019

### IT 관련 자격

- Oracle Cloud Infrastructure Architect / Operations / Foundation
- 리눅스마스터 2급
- PCCE(Python) Lv.1
- E-Test(e-Professionals)

</details>
