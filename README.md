# 문영식 | Youngsik Moon

**고객의 문제를 사업과 연결하고, 기획부터 개발·배포·운영까지 책임지는 Product Engineer입니다.**

B2B 제품 개발, 보안·금융 IT, 직접 사업을 운영한 경험을 바탕으로 무엇을 왜 만들어야 하는지 판단합니다. 작은 조직과 자원이 제한된 환경에서도 필요한 기술을 스스로 익히며 일을 완수해 왔습니다. 개발에 AI를 적극 활용하고, 기술적 판단과 결과 검증은 직접 책임집니다.

[LinkedIn](https://www.linkedin.com/in/moonyoungsik95) · [이메일](mailto:moonyoungsik95@gmail.com)

## 실무 프로젝트

### SmartDash · 기업 업무 통합 B2B SaaS

**와이씨코퍼레이션에서 사업 모델 제안부터 제품 개발·운영, 고객 기술영업까지 주도하고 있습니다.** 그룹웨어, CRM, 견적·수주, 생산·재고, 인사·근태와 설비 데이터를 통합하는 제품입니다.

Odoo 기반 사업을 준비하며 예상되는 도입·운영 문제와 기존 자사 솔루션의 한계를 파악했고, 앞으로의 사업 방향에 맞는 새로운 자사 솔루션을 제안했습니다. 이후 기능 기획, 시스템·UI/UX 설계, 프론트엔드·백엔드 개발, DB·인프라 구성과 배포·운영을 혼자 맡아 진행하고 있습니다.

고객을 직접 만나 데모와 컨설팅을 진행하고 요구사항을 제품에 반영합니다. 기술영업을 진행한 **9개 고객사에서 도입 의향을 확인**했으며, 정부지원사업 선정과 별개로 제품 도입을 희망하는 고객도 생겼습니다.

**핵심 기술:** Python · FastAPI · React · TypeScript · PostgreSQL · AWS

<details>
<summary>기술적 문제 해결 사례</summary>

| 해결한 문제 | 접근과 구현 |
| --- | --- |
| 기능 확장에 따라 흩어지는 업무 규칙 | 모듈러 모놀리식 구조 안에서 업무 경계를 나누고 생산·재고·결재의 공통 정책을 분리 |
| 결재선 조회의 반복 SQL | 관계 데이터 일괄 조회와 키 기반 매핑으로 변경. 격리 재현 테스트에서 SQL 실행 401회 → 5회, 응답 동일성 확인 |
| 동시 요청과 재시도로 인한 데이터 불일치 | 행 잠금, 잠금 순서 통일, 트랜잭션과 멱등 처리 적용 |
| 고객사·사용자별 데이터 접근 통제 | 회사·소유 관계·업무 권한 검사와 서버 세션 검증, 계정 전환 시 조회 캐시 분리 |
| 환경별 DB 변경과 배포 관리 | Alembic 리비전과 GitHub Actions를 연결해 마이그레이션·상태 확인 절차 구성 |
| 외부 메일 연동의 부분 실패 | SMTP 발송 성공과 보낸편지함 저장 실패를 구분해 중복 발송 방지 |

> SQL 수치는 결재선 100개·각 1단계·공통 결재자 조건의 SQLite 격리 재현 결과입니다. 운영 환경의 응답시간 개선율을 뜻하지 않습니다.


</details>

### 그 밖의 실무

| 프로젝트 | 담당한 일 |
| --- | --- |
| **SmartLine2 · MES** | 인수인계 문서 없이 소스와 DB를 분석해 업무 흐름을 파악하고, Spring Boot·React 기반 기능 개선과 운영 담당 |
| **KPI 2.0 · 데이터 수집·전송** | 정부지원사업 OpenAPI를 바탕으로 Python·PySide6·PostgreSQL 기반 스케줄러 기획·설계·개발·운영 |
| **SmartLinePlus** | 자사 MES와 Odoo ERP 연동 및 커스텀 모듈 개발 |
| **MES 장애 복구** | 고객사 실행 장애의 원인 분석, 복구와 재발 방지를 위한 재빌드 |
| **협동로봇 커피머신** | 키오스크·주문 관리 시스템 개발. 로봇 제어를 제외한 소프트웨어 담당 |
| **Fusion 360 KPI 수집** | 데이터 수집·전송 유틸리티 기획·개발·운영 |

## 직접 만든 개인 제품

### BuildBrief · 아이디어를 개발 가능한 기획으로

아이디어는 있지만 구체적으로 설명하거나 AI 개발 도구에 전달하기 어려운 사람을 위해 만들었습니다. 질문에 답하고 화면을 구성하면, 함께 검토할 기획 초안과 AI 전달문으로 정리할 수 있습니다.

현재는 **상용화 전 프로토타입**입니다. 핵심 사용 흐름을 먼저 구현하기 위해 HTML·CSS·JavaScript로 개발했으며, 사용자 피드백에 따라 상용 솔루션으로 발전시킬 계획입니다. 서비스 안에서 AI를 직접 호출하는 방식은 아닙니다.

[사용해 보기](https://buildbrief.moon0sik.cloud/) · [코드와 설계 설명](https://github.com/YoungsikMoon/buildbrief)

### HWPX-HWP 변환기 · 구형 한컴오피스의 문서 호환 문제 해결

한컴오피스 설치나 인터넷 연결 없이 HWPX를 HWP 5.x 문서로 변환하는 Windows 프로그램입니다. Python·PySide6 UI에 오픈소스 변환 엔진을 통합하고, 원본·결과의 좌우 미리보기, 문서 비교 경고와 덮어쓰기 방지를 구현했습니다. 최신 문서 개체는 변환 결과가 달라질 수 있어 직접 비교할 수 있도록 했습니다.

[소스 코드](https://github.com/YoungsikMoon/hwpx-hwp-converter) · [Windows 다운로드](https://github.com/YoungsikMoon/hwpx-hwp-converter/releases/latest)

### CleanFolder · 확인하고 되돌릴 수 있는 파일 정리

확장자·정규식·크기별 사용자 규칙으로 파일을 정리하는 Python·PySide6 데스크톱 프로그램입니다. 실행 전 미리보기와 마지막 작업 되돌리기를 제공하며, Windows 실행 파일과 소스를 공개했습니다.

[소스 코드](https://github.com/YoungsikMoon/CleanFolder) · [Windows 다운로드](https://github.com/YoungsikMoon/CleanFolder/releases/latest)

## 경력과 기술

보안·금융 IT 현장에서 시스템의 안정성과 운영 요구를 익혔고, 직접 사업을 운영하며 재고·매입·지출·근태·급여 관리를 시스템화했습니다. 지금은 그 경험을 고객의 업무와 비용을 이해하는 B2B 제품 개발에 연결하고 있습니다.

| 기간 | 소속·활동 | 주요 경험 |
| --- | --- | --- |
| 2024.11–현재 | 와이씨코퍼레이션 · DX사업본부 수석연구원 / 매니저 | B2B SaaS·MES 기획과 개발, 인프라·운영, PM, 고객 컨설팅과 기술영업 |
| 2022년 시작 | 직접 사업 운영 | 재고·매입·지출·근태·급여 관리 시스템화 및 운영 프로세스 개선 후 사업 정리 |
| 2021.08–2023.02 | 센텍정보기술 · 기술본부 대리 / 매니저 | 금융·기업 고객의 배치 자동화 솔루션 JobMind 구축, POC, 운영과 기술지원 |
| 2019.04–2020.05 | 에스에스앤씨 · 기술본부 대리 / 매니저 | 엔드포인트·스마트팩토리 보안 솔루션 구축과 운영, POC, DB 마이그레이션 |
| 2017.10–2018.02 | 아이디스트 · 프리랜서 | SNS 마케팅 자동화 서비스 판매 페이지 개발, CS와 원격 기술지원 |


<details>
<summary>사용 기술과 적용 영역</summary>

| 영역 | 기술 |
| --- | --- |
| Backend | Python, FastAPI, Java, Spring Boot, SQLAlchemy, Alembic |
| Frontend | React, TypeScript, TanStack Query, Zustand |
| Data & Messaging | PostgreSQL, MS SQL Server, Valkey / Redis, MQTT, InfluxDB |
| Infrastructure | Linux, AWS, Oracle Cloud Infrastructure, Docker, GitHub Actions |
| Desktop & Automation | PySide6, tkinter, Selenium |
| AI 프로젝트 경험 | LLM, NLP, 객체 탐지, STT / TTS, PyTorch |


</details>

## 공개 기록

LinkedIn에는 실무 문제 해결 과정을 운영·보안·비용·사용자 경험의 관점으로 정리합니다. 아래에는 팀 실험과 학습 자료, 그 밖의 공개 작업을 모았습니다. 각 저장소 README에서 역할과 구현 범위를 확인할 수 있습니다.

<details>
<summary>팀 프로젝트·AI 실험</summary>

| 프로젝트 | 내용 |
| --- | --- |
| [InBest](https://github.com/YoungsikMoon/05.-InBest) | 주가·뉴스 분석 팀 프로젝트. 뉴스 수집·분석, LLM 실험과 Streamlit 화면 담당 |
| [Object Detection](https://github.com/YoungsikMoon/04.-ObjectDetection) | 쓰러짐 감지 팀 프로젝트와 사람 탐지 개인 실험 |
| [Find Imo](https://github.com/YoungsikMoon/03.-Find_Imo) | ViT·MLP-Mixer 이미지 모델 연구. AI 면접 적용은 구상 단계 |
| [FORS](https://github.com/YoungsikMoon/02.-FORS) | 음성 인식·LLM 서비스 실험. 음성 데이터 가공과 한국어 모델 실험 참여 |
| [Alpha911](https://github.com/YoungsikMoon/01.-alpha911) | 한·영 웹툰 댓글 수집·전처리·토픽 모델링 |
| [전세버스 서비스 시연](https://www.youtube.com/watch?v=BDou4zE-RDQ) | Java 웹 개발 팀 프로젝트 |

</details>

<details>
<summary>그 밖의 구현·학습·집필</summary>

| 작업 | 내용 |
| --- | --- |
| [CKEditorToPDF](https://github.com/YoungsikMoon/CKEditorToPDF) | Vue·Spring Boot 기반 문서 편집과 Playwright PDF 변환 |
| [YouTube Downloader](https://github.com/YoungsikMoon/youtube-downloader-gui) | Excel 일괄 작업과 실행 로그를 지원하는 Windows GUI 도구 |
| [Secu Book](https://github.com/YoungsikMoon/secu-book) | 커뮤니티와 함께 개선하는 웹 실무 보안 책 |
| [Text Mining](https://github.com/YoungsikMoon/00.-Text-Mining) | 텍스트 전처리·분류 학습 노트 |
| [Spring Security](https://github.com/YoungsikMoon/SpringSecurity) · [Spring JWT](https://github.com/YoungsikMoon/SpringJWT) | 세션·토큰 인증 흐름 학습 |

</details>

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
