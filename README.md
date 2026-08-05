<!--
  GitHub 프로필 README
  사용법: github.com/fraidy53/fraidy53 저장소를 만들고 이 README.md를 푸시하세요.
  (사용자명과 같은 이름의 Public 저장소 → Profile에 자동 표시)
-->

<div align="center">

# 김보민 · Bomin Kim

### Cloud · DevOps · Backend

**배포로 끝내지 않고, 복구까지 설계하는 신입 DevOps 엔지니어를 목표로 합니다.**

[![GitHub](https://img.shields.io/badge/GitHub-fraidy53-181717?style=flat-square&logo=github)](https://github.com/fraidy53)
[![Blog](https://img.shields.io/badge/Blog-bomin27.tistory-FF5722?style=flat-square&logo=tistory&logoColor=white)](https://bomin27.tistory.com)
[![Email](https://img.shields.io/badge/Email-a01051889610@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:a01051889610@gmail.com)

</div>

---

## About Me

수원대학교 정보보호학과에서 개발 기반을 쌓고, **SK쉴더스 루키즈 개발 5기**에서 Cloud/DevOps로 방향을 잡았습니다.

백엔드 요청 흐름을 이해한 뒤 인프라를 설계하고, 장애가 나면 FE → BE → MQ → Consumer → VPN → GPU처럼 **레이어를 따라 원인을 좁히는** 방식으로 일합니다.  
기능이 돌아가는 것보다, 팀이 같은 기준으로 배포·복구할 수 있는 구조를 남기는 일을 중요하게 생각합니다.

| | |
|---|---|
| **Education** | 수원대학교 정보보호학과 · 평점 4.01/4.5 |
| **Training** | SK쉴더스 루키즈 개발 5기 (2026.02–07) · **개인 성적우수 1위** |
| **Focus** | AWS · EKS · GitOps · Terraform · 하이브리드 운영 |

---

## Highlights

- **최우수상 (전체 2위)** — SK쉴더스 루키즈 최종 프로젝트 · ForenShield Cloud/DevOps
- **개인 성적우수 1위** — SK쉴더스 루키즈 개발 5기
- **교내 1위** — FOCUS · 저시력 시각장애인 배달 앱 접근성 위젯
- **중간평가 우수** — 2025 ICT 한이음 드림업 · EUM

---

## Tech Stack

### Cloud / DevOps
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![EKS](https://img.shields.io/badge/Amazon%20EKS-FF9900?style=flat-square&logo=amazonecs&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Argo CD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)

### Backend / Data
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)

---

## Featured Projects

### 1. ForenShield — 안티 딥페이크 디지털 포렌식 플랫폼
**SK쉴더스 루키즈 최종 프로젝트 · 2026.05–07 · 6인 · Cloud/DevOps · 최우수상**

딥페이크 탐지와 증거 무결성 검증을 하나의 운영 가능한 서비스로 연결한 플랫폼입니다.  
FE·BE·AI Consumer를 **AWS EKS**에서 운영하고, 무거운 추론은 **Site-to-Site VPN**으로 온프레미스 GPU에 연결했습니다.

| 내가 한 일 | 내용 |
|---|---|
| **인프라 구축** | VPC·Subnet, EKS Node Group, RDS, S3, Redis, ALB, Route53, IRSA |
| **GitOps** | GitHub Actions → ECR → Manifest → Argo CD → Rollout |
| **하이브리드 연동** | Site-to-Site VPN · GPU Gateway · RabbitMQ 비동기 분석 경로 |
| **운영 자동화** | Terraform·PowerShell 기반 Park/Wake (종료·기동·헬스체크) |
| **무결성 PoC** | 원본·리포트·감사로그 해시를 Hyperledger Fabric에 앵커링 |

**운영에서 배운 점**  
배포 성공 ≠ 복구 완료. Pod Ready, EKS→GPU Health, 외부 HTTPS Health까지 통과해야 완료로 봤습니다.

**Repos**
- [infra-forensic](https://github.com/sk-final-deepfake/infra-forensic) — 인프라 · GitOps · Park/Wake
- [backend-forensic](https://github.com/sk-final-deepfake/backend-forensic) · [ai-forensic](https://github.com/sk-final-deepfake/ai-forensic) · [frontend-deepfake](https://github.com/sk-final-deepfake/frontend-deepfake)
- [트러블슈팅 기록](https://bomin27.tistory.com) — RabbitMQ · VPN · 하이브리드 장애 대응

---

### 2. 사내 프로젝트 관리·결재 통합 시스템 (Mini ERP)
**SK쉴더스 루키즈 미니 프로젝트 · 2026.03–04 · 6인 · Backend**

JWT·RBAC·Redis OTP 기반 인증과 근태 규칙을 구현하고,  
공통 응답·예외·Swagger·Flyway 등 팀이 병렬 개발할 수 있는 기반을 초기에 맞춰 두었습니다.

`Spring Boot` · `Spring Security` · `JPA` · `Redis` · `MariaDB` · `Flyway`

---

### 3. EUM — 저시력 시각장애인 배달 앱 가이드
**2025 ICT 한이음 드림업 · 2025.03–10 · 5인 · Backend 전체 · 중간평가 우수**

인증·소셜 로그인·AI 챗봇·이미지 인식 API를 구현하고,  
RDS · Bedrock · Polly · Rekognition · S3를 연동했습니다.  
IAM·CORS·DTO 불일치를 잡으며 프론트–백엔드 통합을 마무리했습니다.

[EUM_Back](https://github.com/fraidy53/EUM_Back) · `Spring Boot` · `AWS`

---

### 4. University Projects

| Project | Role | Stack | What I learned |
|---|---|---|---|
| **FOCUS** | Flutter/Kotlin · 교내 1위 | Flutter, MethodChannel | 패키지 한계를 네이티브 통신으로 우회 |
| **QuestLog** | Backend | Spring Boot | 재현 가능한 API 테스트 가이드 |
| **SafeRide** | IoT | UART, 센서 | 임계값·디바운싱으로 오작동 개선 |

[FOCUS_GIT](https://github.com/fraidy53/FOCUS_GIT) · [QuestLog_Back](https://github.com/fraidy53/QuestLog_Back)

---

## How I Work

```text
상태 확인 → 경계 구분 → 실패 구간 좁히기 → 설정·경로 조치 → E2E 검증 → 런북·자동화
```

- 증상을 특정 파트 문제로 단정하지 않고, **마지막 정상 구간과 첫 실패 구간**을 기준으로 봅니다.
- 한 번 겪은 장애는 블로그·스크립트·체크리스트로 남겨 같은 실수를 반복하지 않습니다.
- “누가 잘못했나”보다 **확인한 상태**를 먼저 공유하는 협업을 선호합니다.

---

## Currently Learning

- Metrics · Logs · Traces 관측 체계
- SLI/SLO와 알림 기준 설계
- Terraform 모듈화 · 상태 관리
- Kubernetes 네트워크 · 보안 정책

---

## GitHub Stats

<div align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=fraidy53&show_icons=true&theme=transparent&hide_border=true&bg_color=00000000&title_color=24292F&text_color=57606A&icon_color=0969DA" alt="GitHub stats" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=fraidy53&layout=compact&theme=transparent&hide_border=true&bg_color=00000000&title_color=24292F&text_color=57606A" alt="Top languages" />
</div>

---

<div align="center">

**“동작하는 기능”을 넘어, “운영할 수 있는 서비스”를 만들겠습니다.**

`Cloud` · `DevOps` · `Infrastructure` 포지션에 관심 있습니다.  
편하게 연락 주세요.

</div>
