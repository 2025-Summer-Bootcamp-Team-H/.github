<div align="center">

# 🏥 **ClaimBridge** 🏥

### **🤖 AI 기반 보험금 1차 심사 자동화 시스템** 

💡 보험 1차 심사의 패러다임을 바꾼 ClaimBridge을 경험해보세요!

---

</div>

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

### 🖥️ ClaimBridge

> URL : [claimbridge.world](https://claimbridge.world)

### 🔎 ClaimBridge Medium 

> URL

### 주요 기능

* **AI 기반 OCR 처리**: 진단서/영수증 이미지에서 텍스트 자동 추출
* **위조분석**: AI를 통한 문서 위조 여부 분석
* **보험금 계산**: 자동 보험금 계산 및 청구 생성
* **PDF 처리**: 보험 약관 PDF에서 조항 자동 추출
* **관리자 대시보드**: 청구 관리 및 통계 분석
* **실시간 모니터링**: Prometheus, Jaeger를 통한 시스템 모니터링

# 🕺🏻 Demo

### Onboarding

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

### Edit Page

> 병원 영수증 및 진단서에서 OCR로 추출된 내용이 잘못된 경우, 이 페이지에서 직접 수정할 수 있으며, 이미지가 안 보일 경우 돋보기 기능을 통해 확대하여 정확하게 확인할 수 있습니다.

### Management Page

> 관리자는 모든 청구 건을 관리하고 승인/거부할 수 있습니다.

Management

### Report Page

> 차트와 통계를 통해 청구 현황을 분석할 수 있습니다.

Report

# 📗 API

![API Documentation](../api-docs.png)

<a name="-system-architecture"></a>
# 🛠️ System Architecture

![System Architecture](../system.png)

# 🔑 ERD


![Database ERD](../erd-diagram.png)


# 💻 Tech Stack

| Field          | Technology of use                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**   | ![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![Styled Components](https://img.shields.io/badge/Styled%20Components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white) ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white) ![Framer Motion](https://img.shields.io/badge/Framer%20Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white) ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white) ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white) |
| **Backend**    | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F36?style=for-the-badge&logo=sqlalchemy&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white) ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white) ![Anthropic](https://img.shields.io/badge/Anthropic-FF6B35?style=for-the-badge&logo=anthropic&logoColor=white) ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-0078D4?style=for-the-badge&logo=microsoft&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) ![NLTK](https://img.shields.io/badge/NLTK-000000?style=for-the-badge&logo=nltk&logoColor=white) ![Pillow](https://img.shields.io/badge/Pillow-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white) ![Boto3](https://img.shields.io/badge/Boto3-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white) ![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) |
| **DevOps**     | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white) ![Jaeger](https://img.shields.io/badge/Jaeger-000000?style=for-the-badge&logo=jaeger&logoColor=white) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=for-the-badge&logo=opentelemetry&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white) |
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

# 📁 Directory Structure

<details>
<summary>ClaimBridge-Backend</summary>
         
```
🗂️ Backend
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
┃ ┣ 📃 image.py  
┃ ┣ 📃 medical.py  
┃ ┣ 📃 ocr.py  
┃ ┣ 📃 pdf.py  
┃ ┣ 📃 upload.py  
┃ ┗ 📃 __init__.py  

┣ 🗂️ input_pdfs  
┃ ┣ 📃 삼성생명_스마트보장보험.pdf  
┃ ┣ 📃 삼성생명_실손의료비보장보험.pdf  
┃ ┗ 📃 삼성생명_희망사랑보험.pdf  

┣ 🗂️ models  
┃ ┣ 📃 database.py  
┃ ┣ 📃 models.py  
┃ ┣ 📃 schemas.py  
┃ ┗ 📃 __init__.py  

┣ 🗂️ output_results  
┃ ┣ 📃 삼성생명_스마트보장보험_extracted_clauses.json  
┃ ┣ 📃 삼성생명_실손의료비보장보험_extracted_clauses.json  
┃ ┗ 📃 삼성생명_희망사랑보험_extracted_clauses.json  

┣ 🗂️ services  
┃ ┣ 📃 ai_config.py  
┃ ┣ 📃 claim_calculator.py  
┃ ┣ 📃 forgery_detector.py  
┃ ┣ 📃 forgery_service.py  
┃ ┣ 📃 pdf_processor.py  
┃ ┣ 📃 storage_service.py  
┃ ┗ 📃 __init__.py  

┣ 🗂️ tests  
┃ ┣ 📃 test_auth.py  
┃ ┣ 📃 test_claims_api.py  
┃ ┣ 📃 test_claims.py  
┃ ┣ 📃 test_forgery.py  
┃ ┣ 📃 test_models.py  
┃ ┣ 📃 test_pdf.py  
┃ ┣ 📃 test_utils.py  
┃ ┗ 📃 __init__.py  

┣ 🗂️ uploads  
┃ ┣ 🗂️ diagnosis  
┃ ┗ 🗂️ receipts  

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

```

</details>

<details>
<summary>ClaimBridge-Frontend</summary>
         
```
🗂️ frontend
├── 🗂️ .github
│   └── 🗂️ ISSUE_TEMPLATE
├── 🗂️ public
│   └── 📃 robots.txt
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
│   │   └── 📃 GlobalStyle.js
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

|            | 최일우 | 오유민 | 김다현 | 김태수 | 윤일환 | 김수현 |
|------------|:------:|:------:|:------:|:------:|:------:|:------:|
| **Profile** | <img src="../choi.png" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> | <img src="../yoomin_profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> | <img src="../dahyun_profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> | <img src="../taesu_profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> | <img src="../ilhwan_profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> | <img src="../soohyun_profile.jpg" width="130" height="130" style="border-radius: 50%; object-fit: cover;"> |
| **Role**    | Team Leader<br>Frontend<br>DevOps | Frontend<br>UI/UX | Frontend<br>UI/UX | Backend<br>DevOps | Backend<br>DevOps | Backend<br>DevOps |
| **GitHub**  | [@Il-Woo-Choi](https://github.com/Il-Woo-Choi) | [@ohyoom](https://github.com/ohyoom) | [@dadazure](https://github.com/dadazure) | [@gimtaesu399](https://github.com/gimtaesu399) | [@oao03](https://github.com/oao03) | [@SoohyunKim123](https://github.com/SoohyunKim123) |

---

<div align="center">

**ClaimBridge** - AI 기반 보험금 1차 심사 자동화 시스템

더 빠르고 정확한 보험금 심사를 경험해보세요! 🏥✨

</div>
