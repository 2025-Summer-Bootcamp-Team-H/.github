<div align="center">

# 🏥 **ClaimBridge** 🏥

### **AI 기반 보험금 1차 심사 자동화 시스템** 
<br><br>

<img src="../main.png">

<br><br>
💡 보험 1차 심사의 패러다임을 바꾼 ClaimBridge을 경험해보세요!
<br><br>

</div>


<br><br>

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
<br><br>

# 📣 Introduction

### 🖥️ ClaimBridge

> URL : [ClaimBridge.World](https://claimbridge.world)

### 🔎 ClaimBridge Medium 

> URL : [ClaimBridge_Medium](https://medium.com/@ksoohyy/claim-bridge-%EB%B3%B4%ED%97%98-1%EC%B0%A8-%EC%8B%AC%EC%82%AC%EC%9D%98-%ED%8C%A8%EB%9F%AC%EB%8B%A4%EC%9E%84%EC%9D%84-%EB%B0%94%EA%BE%BC-%EC%9E%90%EB%8F%99%ED%99%94-%EC%8B%9C%EC%8A%A4%ED%85%9C-2025-siliconvalley-summer-bootcamp-5a3e33289a58)


### 주요 기능

* **🤖 AI 기반 OCR 처리**: Upstage AI Information Extraction API를 활용한 진단서/영수증 이미지에서 텍스트 자동 추출 및 구조화된 데이터 변환
* **🔍 딥러닝 기반 위조분석**: ResNet18 + ELA(Error Level Analysis) 기술을 활용한 문서 위조 여부 분석 (정확도 93%+)
* **💰 지능형 보험금 계산**: 진단명 키워드 매칭 및 보험상품별 특약 자동 적용을 통한 정확한 보험금 산정
* **📄 AI 기반 PDF 조항 추출**: OpenAI GPT-4를 활용한 보험 약관 PDF에서 특약별 보장내용, 지급금액, 최대한도 자동 추출
* **📊 실시간 관리자 대시보드**: Chart.js 기반 시각화를 통한 청구 현황 분석 및 승인/거부 워크플로우 관리
* **📈 엔터프라이즈급 모니터링**: Prometheus 메트릭 수집, Jaeger 분산 추적, cAdvisor 컨테이너 모니터링을 통한 시스템 성능 실시간 추적
  
<br><br>


# 🕺🏻 Demo

### Onboarding

> ClaimBridge의 간략한 설명을 담고 있습니다.


![제목 없는 동영상 - Clipchamp로 제작 (4)](https://github.com/user-attachments/assets/d66e58ff-42a8-4aa7-86f6-21f86f9e408c)



### Upload Page

> 진단서와 영수증 이미지를 업로드하여 AI 분석을 시작할 수 있습니다.

![upload_video](https://github.com/user-attachments/assets/07778066-730e-4152-9e04-b6149706bdef)



### Analysis Page

> AI가 분석한 결과를 확인하고 보험금 청구를 진행할 수 있습니다.

![제목 없는 동영상 - Clipchamp로 제작 (4) (1)](https://github.com/user-attachments/assets/1d33dd75-93f0-43f0-8455-9f6c8d325589)


### Edit Page

> 병원 영수증 및 진단서에서 OCR로 추출된 내용이 잘못된 경우, 이 페이지에서 직접 수정할 수 있으며, 이미지가 안 보일 경우 돋보기 기능을 통해 확대하여 정확하게 확인할 수 있습니다.

![편집1](https://github.com/user-attachments/assets/fa17040a-57a7-48e7-a434-59b127ad495b)

![제목 없는 동영상 - Clipchamp로 제작 (4) (2)](https://github.com/user-attachments/assets/f84953fd-1291-4e39-9f5d-8062087af7ec)



### Login & Sign up

> JWT 기반 인증을 통해 안전하게 로그인하실 수 있습니다.

![로그인](https://github.com/user-attachments/assets/ab5b08bc-fd97-4d74-9797-46b061cd8095)



### Management Page

> 관리자는 모든 청구 건을 관리하고 승인/거부할 수 있습니다.

Management

### Report Page

> 차트와 통계를 통해 청구 현황을 분석할 수 있습니다.

Report

<br><br>

# 📗 API

![API Documentation](../api-docs.png)

<a name="-system-architecture"></a>

<br><br>

# 🛠️ System Architecture

![System Architecture](../system.png)

<br><br>

# 🔑 ERD


![Database ERD](../erd-diagram.png)



<br><br>


# 💻 Tech Stack

| Field          | Technology of use                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Frontend**   | ![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white) ![Styled Components](https://img.shields.io/badge/Styled%20Components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white) ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white) ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white) ![React Router](https://img.shields.io/badge/React%20Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white) ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white) ![Prettier](https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=prettier&logoColor=white) |
| **Backend**    | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white) ![PyMuPDF](https://img.shields.io/badge/PyMuPDF-0078D4?style=for-the-badge&logo=microsoft&logoColor=white) ![Pillow](https://img.shields.io/badge/Pillow-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Requests](https://img.shields.io/badge/Requests-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Faker](https://img.shields.io/badge/Faker-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| **Database**   | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F36?style=for-the-badge&logo=sqlalchemy&logoColor=white) ![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white) |
| **DevOps**     | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white) ![Google Cloud Platform](https://img.shields.io/badge/Google%20Cloud%20Platform-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white) |
| **Monitoring** | ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white) ![Jaeger](https://img.shields.io/badge/Jaeger-000000?style=for-the-badge&logo=jaeger&logoColor=white) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=for-the-badge&logo=opentelemetry&logoColor=white) ![cAdvisor](https://img.shields.io/badge/cAdvisor-FF6B35?style=for-the-badge&logoColor=white) ![Node Exporter](https://img.shields.io/badge/Node%20Exporter-000000?style=for-the-badge&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F47A20?style=for-the-badge&logo=grafana&logoColor=white) |
| **AI/ML**      | ![OpenAI GPT-4](https://img.shields.io/badge/OpenAI%20GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white) ![Upstage AI](https://img.shields.io/badge/Upstage%20AI-000000?style=for-the-badge&logo=upstage&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white) ![ResNet18](https://img.shields.io/badge/ResNet18-000000?style=for-the-badge&logo=pytorch&logoColor=white) ![ELA Analysis](https://img.shields.io/badge/ELA%20Analysis-000000?style=for-the-badge&logo=opencv&logoColor=white) |


<br><br>


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


<br><br>


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


<br><br>


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


<br><br>


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
