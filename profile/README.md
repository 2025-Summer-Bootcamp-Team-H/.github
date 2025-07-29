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

![API Documentation](../api-docs.png)

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


![Database ERD](../erd-diagram.png)


# 💻 Tech Stack

| Field          | Technology of use                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**   | ![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![Styled Components](https://img.shields.io/badge/Styled%20Components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white) ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white) ![Framer Motion](https://img.shields.io/badge/Framer%20Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white) ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white) ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white) |
| **Backend**    | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F36?style=for-the-badge&logo=sqlalchemy&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white) ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white) ![Anthropic](https://img.shields.io/badge/Anthropic-FF6B35?style=for-the-badge&logo=anthropic&logoColor=white) ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-0078D4?style=for-the-badge&logo=microsoft&logoColor=white) |
| **DevOps**     | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white) ![Jaeger](https://img.shields.io/badge/Jaeger-000000?style=for-the-badge&logo=jaeger&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white) |
| **AI/ML**      | ![OpenAI GPT-4](https://img.shields.io/badge/OpenAI%20GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white) ![Anthropic Claude](https://img.shields.io/badge/Anthropic%20Claude-FF6B35?style=for-the-badge&logo=anthropic&logoColor=white) ![Tesseract OCR](https://img.shields.io/badge/Tesseract%20OCR-000000?style=for-the-badge&logo=tesseract&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white) |
| **Testing**    | ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white) ![Locust](https://img.shields.io/badge/Locust-000000?style=for-the-badge&logo=locust&logoColor=white) ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white) ![Prettier](https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=prettier&logoColor=white) |

# 📊 Monitoring


<table>
<tr>
    <td colspan="2" align="center"><b>cAdvisor</b></td>
  </tr>
  <tr>
    <td><img src="../cadvisor.png" width="100%"></td>
    <td><img src="../cadvisor2.png" width="100%"></td>
  </tr>
         
  <tr>
    <td colspan="2" align="center"><b>FastAPI</b></td>
  </tr>
  <tr>
    <td><img src="../fastapi.png" width="100%"></td>
    <td><img src="../fastapi2.png" width="100%"></td>
  </tr>
         
  <tr>
    <td colspan="2" align="center"><b>Node Exporter</b></td>
  </tr>
  <tr>
    <td><img src="../nodeexporter.png" width="100%"></td>
    <td><img src="../nodeexporter2.png" width="100%"></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><b>PostgreSQL</b></td>
  </tr>
  <tr>
    <td><img src="../postgre.png" width="100%"></td>
    <td><img src="../postgre2.png" width="100%"></td>
  </tr>
         
</table>


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

<details>
<summary>ClaimBridge-Backend</summary>
         
```
🗂️ ClaimBridge-Backend
┣ 📃 Dockerfile  
┣ 📃 Dockerfile.prod  
┣ 📃 main.py  
┣ 📃 README.md  
┣ 📃 requirements.txt  
┣ 📃 resnet18_ela.pth  
┣ 📃 TEAM_GUIDE.md  
┣ 📃 가이드.md  

┣ 🗂️ api  
┃ ┣ 📃 auth.py  
┃ ┣ 📃 claims.py  
┃ ┣ 📃 forgeries.py  
┃ ┣ 📃 medical.py  
┃ ┣ 📃 ocr.py  
┃ ┣ 📃 pdf.py  
┃ ┣ 📃 upload.py  
┃ ┣ 📃 __init__.py  
┃ ┗ 🗂️ __pycache__  
┃   ┣ 📃 auth.cpython-311.pyc  
┃   ┣ 📃 claims.cpython-311.pyc  
┃   ┣ 📃 forgeries.cpython-311.pyc  
┃   ┣ 📃 medical.cpython-311.pyc  
┃   ┣ 📃 ocr.cpython-311.pyc  
┃   ┣ 📃 pdf.cpython-311.pyc  
┃   ┣ 📃 upload.cpython-311.pyc  
┃   ┗ 📃 __init__.cpython-311.pyc  

┣ 🗂️ api_backup  
┃ ┣ 📃 claims.py  
┃ ┣ 📃 medical.py  
┃ ┗ 📃 pdf.py  

┣ 🗂️ input_pdfs  
┃ ┣ 📃 .gitkeep  
┃ ┣ 📃 삼성생명_스마트보장보험.pdf  
┃ ┣ 📃 삼성생명_실손의료비보장보험.pdf  
┃ ┗ 📃 삼성생명_희망사랑보험.pdf  

┣ 🗂️ models  
┃ ┣ 📃 database.py  
┃ ┣ 📃 models.py  
┃ ┣ 📃 schemas.py  
┃ ┣ 📃 __init__.py  
┃ ┗ 🗂️ __pycache__  
┃   ┣ 📃 database.cpython-311.pyc  
┃   ┣ 📃 models.cpython-311.pyc  
┃   ┣ 📃 schemas.cpython-311.pyc  
┃   ┗ 📃 __init__.cpython-311.pyc  

┣ 🗂️ output_results  
┃ ┣ 📃 .gitkeep  
┃ ┣ 📃 삼성생명_스마트보장보험_extracted_clauses.json  
┃ ┣ 📃 삼성생명_실손의료비보장보험_extracted_clauses.json  
┃ ┗ 📃 삼성생명_희망사랑보험_extracted_clauses.json  

┣ 🗂️ services  
┃ ┣ 📃 ai_config.py  
┃ ┣ 📃 claim_calculator.py  
┃ ┣ 📃 forgery_detector.py  
┃ ┣ 📃 forgery_service.py  
┃ ┣ 📃 pdf_processor.py  
┃ ┣ 📃 __init__.py  
┃ ┗ 🗂️ __pycache__  
┃   ┣ 📃 claim_calculator.cpython-311.pyc  
┃   ┣ 📃 forgery_detector.cpython-311.pyc  
┃   ┣ 📃 forgery_service.cpython-311.pyc  
┃   ┣ 📃 pdf_processor.cpython-311.pyc  
┃   ┗ 📃 __init__.cpython-311.pyc  

┣ 🗂️ tests  
┃ ┣ 📃 test_claims.py  
┃ ┗ 📃 __init__.py  

┣ 🗂️ uploads  

┣ 🗂️ utils  
┃ ┣ 📃 auth.py  
┃ ┣ 📃 ela.py  
┃ ┣ 🗂️ scripts  
┃ ┃ ┣ 📃 create_final_dummy_data.py  
┃ ┃ ┣ 📃 ela_dataloader_test.py  
┃ ┃ ┣ 📃 ela_dataset.py  
┃ ┃ ┣ 📃 make_ela_dataset.py  
┃ ┃ ┣ 📃 test_setup.py  
┃ ┃ ┗ 📃 train_resnet18_ela.py  
┃ ┣ 🗂️ sql  
┃ ┃ ┗ 📃 init_database.sql  
┃ ┗ 🗂️ __pycache__  
┃   ┣ 📃 auth.cpython-311.pyc  
┃   ┗ 📃 ela.cpython-311.pyc  

┗ 🗂️ __pycache__  
  ┗ 📃 main.cpython-311.pyc  

🗂️ deploy  
┣ 📃 aws-deploy.sh  
┣ 📃 gcp-deploy.sh  
┗ 📃 배포.md  

🗂️ docs  
┣ 📃 Architecture.md  
┗ 📃 ERD.md  

🗂️ nginx  
┣ 📃 nginx.conf  
┣ 📃 nginx.prod.conf  
┗ 🗂️ ssl  

🗂️ uploads  
┣ 🗂️ diagnosis  
┗ 🗂️ receipts  

```

</details>

<details>
<summary>ClaimBridge-Frontend</summary>
         
```
🗂️ frontend
├── 🗂️ .github
│   └── 🗂️ ISSUE_TEMPLATE
├── 🗂️ node_modules
├── 🗂️ public
├── 🗂️ src
│   ├── 🗂️ assets
│   │   ├── 🗂️ Analysis
│   │   ├── 🗂️ fonts
│   │   ├── 🗂️ Navbar
│   │   ├── 🗂️ Onboarding
│   │   └── 🗂️ Upload
│   ├── 🗂️ components
│   │   ├── 🗂️ buttons
│   │   ├── 📃 Container.jsx
│   │   ├── 📃 LoadingOverlay.jsx
│   │   ├── 📃 Navbar.jsx
│   │   └── 📃 Textinput.jsx
│   ├── 🗂️ config
│   │   └── 📃 api.js
│   ├── 🗂️ hooks
│   │   └── 📃 useAPI.js
│   ├── 🗂️ pages
│   │   ├── 📃 Analysis.jsx
│   │   ├── 📃 Complete.jsx
│   │   ├── 📃 Diagnosis_edit.jsx
│   │   ├── 📃 Login.jsx
│   │   ├── 📃 Management.jsx
│   │   ├── 📃 Onboarding.jsx
│   │   ├── 📃 Receipt_edit.jsx
│   │   ├── 📃 Report.jsx
│   │   ├── 📃 Signup.jsx
│   │   └── 📃 Upload.jsx
│   ├── 🗂️ services
│   │   ├── 📃 apiClient.js
│   │   ├── 📃 authAPI.js
│   │   ├── 📃 claimsAPI.js
│   │   ├── 📃 diagnosisAPI.js
│   │   ├── 📃 forgeryAPI.js
│   │   ├── 📃 index.js
│   │   └── 📃 receiptAPI.js
│   ├── 🗂️ styles
│   ├── 📃 App.jsx
│   └── 📃 main.jsx
├── 📃 .env
├── 📃 .gitignore
├── 📃 .prettierrc
├── 📃 eslint.config.js
├── 📃 index.html
├── 📃 package-lock.json
├── 📃 package.json
├── 📃 README.md
├── 📃 vercel.json
└── 📃 vite.config.js

```
</details>

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
