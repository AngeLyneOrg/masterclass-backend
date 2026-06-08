# ⚙️ Ange Mastery - Intelligent Backend Ecosystem

## 📝 Project Overview
This repository centralizes the infrastructure and server logic for the **Ange Mastery** platform. It relies on a high-performance hybrid architecture combining a robust CMS for content management and an asynchronous server dedicated to real-time Artificial Intelligence services.

### 🌟 Architecture Components
1. **Core Backend & CMS (Django):** Manages secure authentication, course modeling, quiz creation, and data administration via the native admin panel.
2. **AI System Agent (FastAPI):** An isolated asynchronous microservice handling failure predictive algorithms and real-time chat channels via WebSockets.
3. **Database (MongoDB):** A flexible NoSQL database serving as common storage, accessed via the Djongo connector (Django side) and Beanie ODM (FastAPI side).

---

## 🛠️ Tech Stack & Tools
- **Language:** Python 3.11+
- **CMS & Admin Framework:** Django (Powered by the **Djongo** SQL-to-NoSQL connector)
- **API Engine & AI Framework:** FastAPI (Asynchronous non-blocking)
- **Database:** MongoDB (Local Dev & MongoDB Atlas Cloud)
- **AI ODM:** Beanie (Asynchronous Object Document Mapper)
- **Security:** PyJWT (Ephemeral access token management)

---

## 📂 Repository Structure
```text
ange-mastery-backend/
├── masterclass_backend/          # Django core configuration (settings, urls)
├── apps/                         # Django CMS business applications
│   ├── users/                    # Student profiles & Custom Auth
│   ├── courses/                  # Course, module, and video models
│   └── quizzes/                  # MCQ models and administration Inlines
├── ai_agent/                     # Independent FastAPI AI server
│   ├── models/                   # Beanie document schemas
│   └── routers/                  # WebSockets & REST endpoints
└── docker-compose.yml            # Complete environment orchestration
```