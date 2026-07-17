# ⚙️ Car Price Prediction — FastAPI Backend Service

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-Models-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Swagger](https://img.shields.io/badge/Swagger-OpenAPI-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

An asynchronous, high-performance REST API built with **FastAPI** to serve machine learning predictions for used car prices. It features dynamic model fetching from the **Hugging Face Hub**, input validation, and containerization with **Docker** for cloud deployment.

---

## 🔗 Live Services & Links

* ⚙️ **Interactive API Docs (Swagger):** [Swagger Documentation](https://car-prediction-backend-production.up.railway.app/docs)
* 🌐 **Frontend Application:** [Car Prediction Web App](https://car-prediction-reactjs.vercel.app/)
* 🤖 **Hugging Face Model Hub:** [Car Prediction ML Model](https://huggingface.co/Hossam-27/car-prediction-ml-model/tree/main)
* 📦 **Full System Repository:** [Car Prediction Full Project](https://github.com/hossam-ibrahim27/car-prediction-full-project)

---

## 📁 Repository Structure

```text
predict_backend/
├── 📁 models/            # Cached machine learning artifacts & pipelines
├── Dockerfile            # Container deployment configuration
├── main.py               # FastAPI application, endpoints & CORS config
├── requirements.txt      # Python dependencies
└── upload_huggingface.py # Automated script to push trained pipelines to Hugging Face
```

```text
 ┌──────────────────────┐        ┌──────────────────────┐        ┌──────────────────────┐
 │  HTTP POST Request   │ ────>  │ FastAPI REST Engine  │ ────>  │  Hugging Face Hub    │
 │ (Vehicle Features)   │        │ (Pydantic Validation)│        │ (Model Artifacts)    │
 └──────────────────────┘        └──────────────────────┘        └──────────────────────┘
 ```

 ### 1. API Core & Validation
* **FastAPI:** Asynchronous Python web framework providing rapid response times and OpenAPI standard compliance.
* **Pydantic:** Strict runtime type validation and schema enforcement for request payloads.

### 2. Machine Learning & Model Fetching
* **Hugging Face Hub:** Cloud storage integration to dynamically fetch pre-trained Scikit-Learn pipelines on startup.
* **Pipeline Inference:** Deserializes trained feature transformers and regression models to serve real-time predictions.

### 3. Deployment & Infrastructure
* **Docker:** Multi-stage Dockerized environment ensuring seamless deployment across cloud providers.
* **CORS Middleware:** Configured cross-origin resource sharing to securely serve requests from the React frontend.
  
---

## 🔒 License & Intellectual Property

Copyright (c) 2026 Hossam Ibrahim. All Rights Reserved.

This repository and its source code are published for showcase, code review, and portfolio evaluation purposes only. No part of this software may be copied, modified, distributed, or used for commercial purposes without prior written permission from the owner.
