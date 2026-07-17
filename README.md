# 🚗 Car Price Prediction System

![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-131415?style=for-the-badge&logo=railway&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

An end-to-end Machine Learning web application engineered to predict used car prices in real-time based on vehicle specifications such as manufacturing year, mileage, fuel type, transmission, and engine capacity.

---

## 🔗 Live Demos & Links

* 🌐 **Frontend App (Vercel):** [https://your-app.vercel.app](https://your-app.vercel.app)
* 📄 **Interactive API Docs (Swagger UI):** [https://car-prediction-backend-production.up.railway.app/docs](https://car-prediction-backend-production.up.railway.app/docs)
* 📦 **Model Storage (Hugging Face):** [Hossam-27/car-prediction-ml-model](https://huggingface.co/Hossam-27/car-prediction-ml-model)

---

## 🛠️ Tech Stack & Architecture

* **Machine Learning:** Scikit-Learn (Random Forest & Linear Regression, StandardScaler, One-Hot Encoding).
* **Backend:** FastAPI, Uvicorn, Pydantic, Git LFS.
* **Frontend:** React.js, Tailwind CSS, Axios.
* **DevOps & Containerization:** Docker, Railway (Backend API), Vercel (Frontend Hosting).

---

## 🚀 Key Features

* ⚡ **Real-Time Inference:** Ultra-fast REST API responses powered by FastAPI and Uvicorn.
* 🔄 **Automated Preprocessing Pipeline:** Continuous feature encoding and scaling using serialized `.pkl` pipelines.
* 🐳 **Containerized Deployment:** Dockerized backend ensuring reliable execution across cloud platforms.
* 🛡️ **Robust Data Validation:** Strictly typed API endpoints leveraging Pydantic schemas.

---

## 🔌 API Reference

### `POST /predict`

Calculates the estimated price for a car based on input features.

#### Request Body
```json
{
  "year": 2018,
  "mileage": 85000,
  "fuel_type": "Petrol",
  "transmission": "Automatic",
  "engine_size": 2.0
}
#### Response (200 OK)
```json
{
  "status": "success",
  "predicted_price": 14500.00,
  "currency": "USD"
}
