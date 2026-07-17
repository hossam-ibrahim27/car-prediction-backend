## 🚗 Car Price Prediction API

### 📌 Overview
An end-to-end Machine Learning web application designed to predict used car prices based on key vehicle features such as year, mileage, brand, transmission type, fuel type, and engine capacity.

---

### 🛠️ Tech Stack & Architecture
* **Machine Learning:** Scikit-Learn (Linear Regression & Random Forest Models, Standard Scaler, One-Hot Encoders).
* **Backend:** FastAPI, Uvicorn, Docker.
* **Frontend:** React.js, Tailwind CSS.
* **Deployment & Hosting:** 
  * Model Storage: Hugging Face Model Hub (`Hossam-27/car-prediction-ml-model`)
  * Backend API: Render / Hugging Face Spaces (Docker Container)
  * Frontend: Vercel

---

### 🚀 Key Features
* **Real-time Inference:** Fast REST API response times powered by FastAPI.
* **Data Preprocessing Pipeline:** Automated feature encoding and scaling using pre-trained `.pkl` artifacts.
* **Containerized Deployment:** Packaged using Docker for consistent cross-environment performance.

---

### 🔌 API Endpoints

#### `POST /predict`
Sends car parameters and receives the estimated price.

**Sample Request Body:**
```json
{
  "year": 2018,
  "mileage": 85000,
  "fuel_type": "Petrol",
  "transmission": "Automatic",
  "engine_size": 2.0
}
