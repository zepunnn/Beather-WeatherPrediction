# 🌦️ Beather: Weather Prediction Project for Batang, Central Java, Indonesia

![Project Status](https://img.shields.io/badge/Status-On--Progress-yellow)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Machine Learning](https://img.shields.io/badge/AI-Scikit--Learn-orange)
![License](https://img.shields.io/badge/License-MIT-green)

> **Delivering hyper-local weather intelligence for Batang, Central Java — powered by Machine Learning and real-time BMKG Open Data.**

---

## 📖 Overview

**Beather (Batang Weather)**—also known internally as **BatangCast**—is a weather prediction platform built to deliver accurate, ML-driven forecasts for the **Batang Regency** region.

Unlike generic applications that only provide city-level weather information, Beather focuses on **Kelurahan/Desa-level predictions**, enabling a far more precise and actionable forecast for residents, farmers, fishermen, and daily commuters.

This system transforms complex meteorological datasets from **BMKG** into meaningful predictions through an automated pipeline, from data ingestion to prediction serving.

---

## ✨ Key Features

* **📍 Hyper-Local Forecasting:** View predictions filtered down to specific **Kelurahan/Desa** within Batang Regency.
* **🤖 AI-Powered Predictions:** Machine Learning models identify rainfall likelihood and weather patterns using historical BMKG data.
* **📊 Interactive Visualization:** Dynamic, user-friendly charts (Chart.js) for understanding weather trends.
* **⚡ Fast & Modern API:** Backend built with **FastAPI**, offering high performance and async capability.
* **🔄 Automated ETL Pipeline:** Continuous synchronization with BMKG Open Data to keep the system up to date.

---

## 🏗️ Tech Stack

This project uses a **decoupled architecture** to ensure scalability, clean data flow, and maintainability.

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Backend & API** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) **FastAPI** | Handles requests, serves ML predictions, manages preprocessing. |
| **Machine Learning** | **Pandas & Scikit-Learn** | Data pipeline, feature extraction, model training & evaluation. |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-005C84?style=flat&logo=mysql&logoColor=white) **MySQL** | Stores historical BMKG weather data and prediction logs. |
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) | Provides UI for choosing locations and viewing weather graphs. |
| **Visualization** | **Chart.js** | Renders interactive charts for temperature, rainfall, and trends. |

---

## 🚀 How It Works

1. **Data Ingestion:** BMKG Open Data is fetched and stored into the MySQL database via automated scripts.
2. **Data Processing:** Backend scripts preprocess and clean the dataset for ML training.
3. **Prediction Serving:** When a user selects a *Kelurahan*, FastAPI loads the trained model and performs inference.
4. **Result Presentation:** The API returns weather predictions, visualized instantly on the frontend.

---

## 🧠 Model & Dataset

* **Dataset Source:** [BMKG Open Data](https://data.bmkg.go.id/)
* **Features:** Temperature, Humidity, Wind Speed, Rainfall Indicators.
* **Model Types:**  
  * **Rain Classification** — RandomForestClassifier  
  * **General Weather Trend** — RandomForestRegressor  
* **Training Workflow:** Periodically retrained using accumulated BMKG historical data.

---

## 🤝 Contributing

Contributions are welcome!  
Developers, data enthusiasts, or anyone passionate about weather modeling in Indonesia are encouraged to fork this repository and submit Pull Requests.

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for details.

---

<p align="center">
  Made with ❤️ for <b>Batang, Indonesia</b>
</p>
