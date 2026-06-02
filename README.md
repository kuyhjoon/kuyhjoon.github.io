<div align="center">

# 손준혁 · Son Junhyuk

### 작동하는 코드보다 **신뢰받는 시스템**을 만드는 Java 백엔드 개발자
### *Java Backend Developer — building systems people can trust, not just code that runs*

<br>

![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

<br>

![Status](https://img.shields.io/badge/Status-Open_to_Opportunities-059669?style=flat-square)
![Experience](https://img.shields.io/badge/Backend-4%2B_years-0369a1?style=flat-square)
![Total Career](https://img.shields.io/badge/Total_Career-7%2B_years-475569?style=flat-square)
![Location](https://img.shields.io/badge/Based_in-Korea-6d28d9?style=flat-square)

<br>

### 🔗 [**라이브 포트폴리오 보기 / View Live Portfolio →**](https://YOUR-USERNAME.github.io)

<sub>다크/라이트 테마 · 완전 반응형 · 의존성 0 · 단일 HTML 파일</sub>
<br>
<sub>Dark/Light theme · Fully responsive · Zero dependencies · Single HTML file</sub>

</div>

---

## 👋 소개 · About

> **"데이터가 안정적으로 흐르는 구조를 설계합니다."**

유전자 분석 장비 연동부터 ERP 자동화, 수십만 건의 광고 성과 리포트까지 —
도메인은 달랐지만 본질은 하나였습니다: **"데이터의 흐름과 상태를 어떻게 안전하게 설계할 것인가?"**

> *From genomics instrument integration to ERP automation and large-scale ad-performance reporting —*
> *the domains differ, but the question is always the same: how do you design data flow and state so it stays reliable?*

응용통계학 석사(GPA 4.35)의 데이터 중심 사고와, 미국 18개월 근무·연수로 다진 글로벌 역량을 바탕으로
**오류 0건 · 가용성 99%+** 를 *코드가 아닌 구조로* 달성하는 데 집중합니다.

---

## 📊 Impact at a Glance · 핵심 성과

| 지표 · Metric | 수치 | 내용 · Context |
|---|:---:|---|
| ⚡ **처리 시간 단축** · Processing time | **95%** | 결과지 생성 20분 → 1분 이내 *(Gaia Report Web)* |
| 💰 **인프라 비용 절감** · Infra cost | **46%** | AWS 리팩토링 + Docker CI/CD *(EC2 리사이징·리소스 통합)* |
| 🤖 **수작업 자동화** · Manual work | **70%** | 리포트 자동 생성 *(제노코어비에스)* |
| 🛡️ **서비스 가용성** · Availability | **99%+** | ELB + Nginx 이중화 *(단일 장애점 제거)* |
| 📦 **핵심 프로젝트 납품** · Projects shipped | **6+** | 전사 시스템 신규 구축·운영 |
| 🔒 **동기화 오류** · Sync errors | **0건** | 명시적 State 관리 + 방어 로직 *(Array LIMS)* |

---

## 🚀 Featured Projects · 주요 프로젝트

### 🧬 Array LIMS — 유전자 분석 장비 연동 시스템
`Java` `Spring Boot` `WebSocket` `CompletableFuture` `Azure OAuth2` `AOP` `MS SQL Server`

GeneTitan 분석 장비의 대용량 실험 데이터를 **실시간 수집·동기화**하는 Microarray LIMS 신규 구축.
- Run 상태를 `QUEUED → RUNNING → COMPLETED / FAILED / RETRY` 로 **명시적 State 관리**
- `CompletableFuture` 비동기 파이프라인 + 독립 스레드 풀 분리로 장비 응답성 유지
- `GlobalExceptionHandler` + `BusinessException` 계층으로 예외 흐름 일원화 → **운영 동기화 오류 0건**

### 📄 Gaia Report Web — 유전자 분석 결과지 플랫폼
`Java` `Spring Boot` `Spring Security` `RBAC / Menu ACL` `AOP Audit` `모듈화 아키텍처`

수작업 결과지 프로세스를 완전 대체하는 사내 웹 플랫폼.
- 역할이 아닌 **메뉴·기능 단위 RBAC** 설계 → 조직 개편 시 *코드 수정 없이* 권한 재구성
- `@Audited` 기반 AOP Audit으로 행위·데이터 변경 이력 자동 추적
- **처리 시간 95% 단축 (20분 → 1분 이내)**

### 🛒 COS — 주문·결제 백오피스
`Java` `Spring Boot` `State Machine` `이벤트 소싱` `AOP`

주문 상태 전이를 **State Machine**으로 명시화해 비정합 주문을 원천 차단,
이벤트 소싱으로 현재 상태 조회와 전체 이력 추적을 동시 지원 → 처리 시간 약 30% 단축.

### 🔁 LESS — ERP 연동 자동화 플랫폼
`Java` `Spring Boot` `트랜잭션 관리` `재시도 패턴` `데이터 정합성`

연동 전·후 **이중 Validation**으로 불완전 데이터의 ERP 반영을 구조적으로 차단,
실패 시 트랜잭션 롤백 + 재시도 패턴으로 반복 업무 약 40% 절감.

### ☁️ AWS 인프라 리팩토링 — DevOps
`AWS EC2/S3/ELB` `Docker` `Nginx` `Redis` `GitHub + rsync CI/CD`

한국/미국 법인 포함 다수 웹사이트 인프라 전면 개선.
EC2 리사이징 · ELB+Nginx 이중화 · Redis 캐싱 · CI/CD 자동화로
**운영 비용 46% 절감 · 가용성 99%+ 달성**.

> 🔍 전체 프로젝트와 상세 내용은 [**라이브 포트폴리오**](https://YOUR-USERNAME.github.io)에서 확인하세요.

---

## 🛠 Tech Stack · 기술 스택

**Backend**
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-DC382D?style=flat-square)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)

**설계 패턴 · Design Patterns**
`State Machine` · `GlobalExceptionHandler` · `RBAC / Menu ACL` · `이벤트 소싱` · `재시도 패턴` · `모듈화 아키텍처`

**Database**
![MS SQL Server](https://img.shields.io/badge/MS_SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle_SQL-F80000?style=flat-square&logo=oracle&logoColor=white)

**DevOps**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Studying** 📚
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![JPA](https://img.shields.io/badge/JPA_/_Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)

---

## 📂 이 저장소는? · About This Repository

이 저장소는 위 내용을 담은 **개인 포트폴리오 웹사이트의 소스 코드**입니다.
*This repository contains the source code of the personal portfolio website above.*

**기술적 특징 · Technical Highlights**
- 🪶 **의존성 0 / Zero dependencies** — 빌드 도구·프레임워크 없이 순수 HTML·CSS·Vanilla JS
- 📦 **단일 파일 / Single file** — 모든 마크업·스타일·스크립트가 [`index.html`](index.html) 하나에
- 🌗 **자동 테마 / Auto theme** — OS 설정 감지 + 수동 토글 (CSS Custom Properties 기반)
- ✨ **스크롤 애니메이션 / Scroll reveal** — `IntersectionObserver` 기반 (라이브러리 없음)
- 📱 **완전 반응형 / Fully responsive** — 모바일·태블릿·데스크톱 대응
- ♿ **접근성 / Accessibility** — 시맨틱 마크업 · `aria` 속성 · 키보드 내비게이션 · `:focus-visible`

---

## 🗂 프로젝트 구조 · Structure

```
portfolio/
├── index.html      # 포트폴리오 본체 (HTML + CSS + JS 단일 파일)
├── assets/         # 이미지·이력서 PDF 등 정적 리소스
└── README.md       # 현재 문서
```

---

## ▶️ 로컬 실행 & 배포 · Run & Deploy

**로컬에서 보기 / View locally**
```bash
# 1) 저장소 클론
git clone https://github.com/YOUR-USERNAME/portfolio.git
cd portfolio

# 2) 브라우저로 바로 열기 (빌드 불필요)
open index.html          # macOS
# 또는 간단한 로컬 서버
python3 -m http.server 8000   # → http://localhost:8000
```

**GitHub Pages 배포 / Deploy**
> `Settings → Pages → Source: main 브랜치 / 루트(/)` 선택 시
> `https://YOUR-USERNAME.github.io/portfolio` 로 자동 배포됩니다.

---

## ✏️ 커스터마이징 체크리스트 · Setup Checklist

`index.html` 내 아래 플레이스홀더를 실제 값으로 교체하세요.
*Replace these placeholders in `index.html` with your real values.*

- [ ] `YOUR-USERNAME` — GitHub 사용자명 (Hero 버튼 · Contact 카드)
- [ ] `your@email.com` — 이메일 주소 (`EMAIL` 변수 + Contact 카드)
- [ ] `YOUR_RESUME.pdf` — 이력서 PDF 경로 (`assets/`에 업로드 후 연결)
- [ ] `YOUR-BLOG-URL` — 기술 블로그 링크
- [ ] `YOUR-PROFILE` — LinkedIn 프로필 링크
- [ ] README 상단 라이브 데모 URL — `https://YOUR-USERNAME.github.io`

---

## 📬 Contact · 연락처

<div align="center">

새로운 기회에 열려 있습니다. 편하게 연락 주세요 · *Open to new opportunities — feel free to reach out.*

[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your@email.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YOUR-USERNAME)
[![Blog](https://img.shields.io/badge/Blog-FF5722?style=for-the-badge&logo=rss&logoColor=white)](https://YOUR-BLOG-URL)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-PROFILE)

<br>
<sub>© 2026 손준혁 · Designed & Built by 손준혁</sub>

</div>
