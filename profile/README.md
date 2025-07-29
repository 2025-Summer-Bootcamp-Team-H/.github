# 🏆 2024 Techeer Summer BootCamp Project 🏆

# 🏥 ClaimBridge 🏥

### **AI 기반 보험금 청구 처리 시스템** 

> **ClaimBridge를 통해 더 빠르고 정확한 보험금 청구를 경험해보세요!**

# 📖 Table of contents

* [Introduction](#-introduction)
* [Demo](#-demo)
* [API](#-api)
* [System Architecture](#-system-architecture)
* [ERD](#-erd)
* [Tech Stack](#-tech-stack)
* [Monitoring](#-monitoring)
* [How to start](#-how-to-start)
* [Directory Structure](#-directory-structure)
* [Team Members](#-team-members)

# 📣 Introduction

### URL

> 🖥️ ClaimBridge

### Medium

> 🔎 ClaimBridge Medium 

### 주요 기능

* **AI 기반 OCR 처리**: 진단서/영수증 이미지에서 텍스트 자동 추출
* **위조분석**: AI를 통한 문서 위조 여부 분석
* **보험금 계산**: 자동 보험금 계산 및 청구 생성
* **PDF 처리**: 보험 약관 PDF에서 조항 자동 추출
* **관리자 대시보드**: 청구 관리 및 통계 분석
* **실시간 모니터링**: Prometheus, Jaeger를 통한 시스템 모니터링

# 🕺🏻 Demo

### Onboarding Page

> ClaimBridge의 간략한 설명을 담고 있습니다.

Onboarding

### Login & Sign up

> JWT 기반 인증을 통해 안전하게 로그인하실 수 있습니다.

Login & Sign up

### Upload Page

> 진단서와 영수증 이미지를 업로드하여 AI 분석을 시작할 수 있습니다.

Upload

### Analysis Page

> AI가 분석한 결과를 확인하고 보험금 청구를 진행할 수 있습니다.

Analysis

### Management Page

> 관리자는 모든 청구 건을 관리하고 승인/거부할 수 있습니다.

Management

### Report Page

> 차트와 통계를 통해 청구 현황을 분석할 수 있습니다.

Report

# 📗 API

![API Documentation](api-docs.png)

# 🛠️ System Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   Backend       │    │   Database      │
│   (React)       │◄──►│   (FastAPI)     │◄──►│   (PostgreSQL)  │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Nginx         │    │   AI Services   │    │   Monitoring    │
│   (Reverse      │    │   (OpenAI,      │    │   (Prometheus,  │
│    Proxy)       │    │    Claude)      │    │    Jaeger)      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

# 🔑 ERD

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│     Users       │    │     Claims      │    │   Documents     │
├─────────────────┤    ├─────────────────┤    ├─────────────────┤
│ id (PK)         │    │ id (PK)         │    │ id (PK)         │
│ email           │    │ user_id (FK)    │    │ claim_id (FK)   │
│ password_hash   │    │ amount          │    │ file_path       │
│ role            │    │ status          │    │ document_type   │
│ created_at      │    │ created_at      │    │ created_at      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       │
         └───────────────────────┼───────────────────────┘
                                 │
                    ┌─────────────────┐
                    │  Medical Info   │
                    ├─────────────────┤
                    │ id (PK)         │
                    │ claim_id (FK)   │
                    │ diagnosis       │
                    │ treatment       │
                    │ cost            │
                    └─────────────────┘
```

# 💻 Tech Stack

| Field          | Technology of use                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**   | ![React](https://img.shields.io/badge/React-19.1.0-blue.svg) ![Vite](https://img.shields.io/badge/Vite-7.0.3-purple.svg) ![Styled Components](https://img.shields.io/badge/Styled%20Components-6.1.19-pink.svg) ![Chart.js](https://img.shields.io/badge/Chart.js-4.5.0-orange.svg) ![Framer Motion](https://img.shields.io/badge/Framer%20Motion-12.23.6-green.svg) ![Axios](https://img.shields.io/badge/Axios-1.10.0-yellow.svg) ![React Router](https://img.shields.io/badge/React%20Router-7.6.3-red.svg) |
| **Backend**    | ![FastAPI](https://img.shields.io/badge/FastAPI-0.109.1-green.svg) ![Python](https://img.shields.io/badge/Python-3.11+-blue.svg) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-2.0.23-red.svg) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue.svg) ![JWT](https://img.shields.io/badge/JWT-PyJWT-orange.svg) ![OpenAI](https://img.shields.io/badge/OpenAI-1.3.7-green.svg) ![Anthropic](https://img.shields.io/badge/Anthropic-0.7.7-purple.svg) ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-1.23.8-blue.svg) |
| **DevOps**     | ![Docker](https://img.shields.io/badge/Docker-Compose-orange.svg) ![Nginx](https://img.shields.io/badge/Nginx-Reverse%20Proxy-green.svg) ![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-red.svg) ![Jaeger](https://img.shields.io/badge/Jaeger-Tracing-blue.svg) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-purple.svg) ![Vercel](https://img.shields.io/badge/Vercel-Deployment-black.svg) |
| **AI/ML**      | ![OpenAI GPT-4](https://img.shields.io/badge/OpenAI%20GPT--4-Language%20Model-green.svg) ![Anthropic Claude](https://img.shields.io/badge/Anthropic%20Claude-AI%20Assistant-purple.svg) ![Tesseract OCR](https://img.shields.io/badge/Tesseract%20OCR-Text%20Recognition-blue.svg) ![OpenCV](https://img.shields.io/badge/OpenCV-Image%20Processing-green.svg) ![PyTorch](https://img.shields.io/badge/PyTorch-Machine%20Learning-orange.svg) |
| **Testing**    | ![Pytest](https://img.shields.io/badge/Pytest-Testing-green.svg) ![Locust](https://img.shields.io/badge/Locust-Load%20Testing-blue.svg) ![ESLint](https://img.shields.io/badge/ESLint-Code%20Quality-purple.svg) ![Prettier](https://img.shields.io/badge/Prettier-Code%20Formatting-pink.svg) |

# 📊 Monitoring

### Prometheus
- 시스템 메트릭 수집
- API 응답 시간 모니터링
- 데이터베이스 성능 추적

### Jaeger (OpenTelemetry)
- 분산 추적
- API 호출 체인 분석
- 성능 병목 지점 식별

### cAdvisor
- 컨테이너 리소스 사용량 모니터링
- Docker 컨테이너 성능 추적

# 🚀 How to start

### 1. 프로젝트 클론
```bash
git clone https://github.com/your-username/claimbridge.git
cd claimbridge
```

### 2. Backend 설정 및 실행

```bash
# Backend 디렉토리로 이동
cd backend

# 환경변수 설정
cp env.example .env
# .env 파일에서 실제 API 키 등으로 수정

# Docker Compose로 실행
docker-compose up -d --build

# 더미데이터 생성 (선택사항)
docker exec -it insurance_backend python utils/scripts/create_final_dummy_data.py
```

### 3. Frontend 설정 및 실행

```bash
# Frontend 디렉토리로 이동
cd frontend

# 의존성 설치
npm install

# 환경변수 설정
echo "VITE_API_BASE_URL=http://localhost:8000/api/v1" > .env

# 개발 서버 실행
npm run dev
```

### 4. 접속 확인

- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:8000
- **API 문서**: http://localhost:8000/docs
- **pgAdmin**: http://localhost:8080 (admin@insurance.com / admin123)

# 📁 Directory Structure

```
claimbridge/
├── backend/                    # 백엔드 서버
│   ├── backend/               # FastAPI 애플리케이션
│   │   ├── api/              # API 엔드포인트
│   │   │   ├── auth.py       # 인증 API
│   │   │   ├── upload.py     # 파일 업로드 API
│   │   │   ├── ocr.py        # OCR 처리 API
│   │   │   ├── claims.py     # 보험금 청구 API
│   │   │   ├── medical.py    # 의료 정보 API
│   │   │   ├── forgeries.py  # 위조분석 API
│   │   │   └── pdf.py        # PDF 처리 API
│   │   ├── models/           # 데이터베이스 모델
│   │   ├── services/         # 비즈니스 로직
│   │   ├── utils/            # 유틸리티/스크립트
│   │   └── main.py           # FastAPI 앱 설정
│   ├── nginx/                # Nginx 설정
│   ├── deploy/               # 배포 스크립트
│   ├── docker-compose.yml    # 개발용 Docker 설정
│   ├── docker-compose.prod.yml # 프로덕션용 Docker 설정
│   └── uploads/              # 업로드 파일 저장소
├── frontend/                  # 프론트엔드 애플리케이션
│   ├── src/
│   │   ├── components/       # 재사용 가능한 컴포넌트
│   │   ├── pages/           # 페이지 컴포넌트
│   │   ├── assets/          # 정적 파일
│   │   ├── styles/          # 전역 스타일
│   │   └── utils/           # 유틸리티 함수
│   ├── package.json         # 의존성 관리
│   └── vite.config.js       # Vite 설정
└── README.md                # 프로젝트 문서
```

# 👥 Team Members

| Name    | 역할                                        | 담당 영역                                    |
| ------- | ------------------------------------------ | -------------------------------------- |
| 팀원 1  | Leader, Backend, Frontend, DevOps          | 전체 시스템 설계 및 개발                    |
| 팀원 2  | Backend, DevOps                            | AI 서비스 및 인프라 구축                   |
| 팀원 3  | Backend, DevOps                            | 데이터베이스 및 API 개발                   |
| 팀원 4  | Frontend, Design                           | 사용자 인터페이스 및 UX 디자인             |
| 팀원 5  | Frontend, Design                           | 프론트엔드 개발 및 컴포넌트 설계           |
| 팀원 6  | Frontend, Design                           | 차트 및 데이터 시각화                      |

---

<div align="center">

**ClaimBridge** - AI 기반 보험금 청구 처리 시스템

더 빠르고 정확한 보험금 청구를 경험해보세요! 🏥✨

</div>
