# 🌱 Tomato Smart Farming – AI-Based Plant Growth Stage and Development Prediction

## 📌 Project Overview

Tomato Smart Farming is an intelligent agriculture application designed to help farmers monitor tomato plant growth, identify visible plant health problems, and make better farming decisions using image analysis, weather information, and predictive insights.

The system aims to simplify crop monitoring by allowing farmers to upload tomato plant photographs and receive information about the plant's growth stage, visible defects, and recommended care practices.

## 🎯 Objectives

- Automatically identify tomato plant growth stages from uploaded images.
- Detect visible plant defects and potential health problems.
- Provide practical recommendations to improve plant health.
- Monitor environmental conditions using location-based weather information.
- Predict upcoming growth stages and estimated development periods.
- Maintain individual plant growth histories.
- Support monitoring of multiple plants and larger farms.

## 🌿 Tomato Growth Stage Classification

The application is designed to classify tomato plants into five major growth stages:

1. **Seedling** – Early development of the young tomato plant.
2. **Vegetative** – Development of stems, leaves, and branches.
3. **Flowering** – Formation and development of flowers.
4. **Fruit Development** – Formation and enlargement of tomato fruits.
5. **Fruit Ripening** – Tomatoes gradually mature and change colour.

## 🔍 Plant Health Analysis

The image-analysis functionality aims to identify visible symptoms such as:

- Yellowing leaves
- Leaf spots and blight-like symptoms
- Wilting
- Stunted growth
- Flower drop
- Poor fruit development
- Visible pest damage
- Damaged fruits

Based on supported findings, the application provides:
- Identified problem
- Severity level
- Recommended treatment
- Preventive measures

Image-based findings are intended as preliminary guidance and not a replacement for laboratory diagnosis or expert agricultural advice.

## 🌦️ Weather Monitoring

The application uses location-based weather information to provide:

- Current temperature
- Humidity
- Rainfall and precipitation
- Wind conditions
- Weather conditions
- Seven-day weather forecasts

Weather information can support the assessment of environmental risks affecting tomato growth.

## 📈 Growth Prediction

The system aims to provide:
- Current growth-stage information
- Expected upcoming growth stages
- Estimated development periods
- Growth progress monitoring
- Weather-related risk insights

Predictions are estimates and may vary depending on tomato variety, environmental conditions, and cultivation practices.

## 🪴 Plant Management

- Add and manage individual tomato plants.
- Monitor multiple plants.
- Maintain plant growth histories.
- Track plant health assessments.
- Archive plants without permanently deleting their records.
- Restore archived plants when required.

## 🛠️ Technologies Used

### Frontend
- React.js
- Vite
- JavaScript
- CSS

### Backend
- Python
- FastAPI
- Uvicorn

### Database and Data Handling
- SQLAlchemy
- PostgreSQL
- Psycopg

### Image Analysis and AI
- Deep Learning
- Computer Vision
- Image Classification
- Pretrained Model Integration

### Weather Integration
- Open-Meteo Weather API
- Browser Geolocation API

## 📂 Project Structure

```text
tomato-smart-farming/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── database/
│   │   ├── schemas/
│   │   └── services/
│   └── requirements.txt
│
├── ai_models/
│   ├── growth_stage/
│   ├── plant_health/
│   ├── growth_forecasting/
│   └── farm_detection/
│
├── datasets/
├── research/
├── storage/
└── tests/
```

## 🚀 Installation and Setup

### Prerequisites

- Python 3.10 or later
- Node.js and npm
- PostgreSQL (if using the PostgreSQL database configuration)
- Visual Studio Code

### 1. Clone the Repository

```bash
git clone YOUR_REPOSITORY_URL
cd tomato-smart-farming
```

### 2. Start the Backend

```bash
cd backend
python -m venv venv
```

Activate the virtual environment on Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start FastAPI:

```bash
uvicorn app.main:app --reload
```

Backend:

```text
http://127.0.0.1:8000
```

API documentation:

```text
http://127.0.0.1:8000/docs
```

### 3. Start the Frontend

Open a separate terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local application at:

```text
http://localhost:5173
```

## 🔮 Future Enhancements

- Improved five-stage tomato growth classification.
- More accurate plant disease and pest detection.
- YOLO-based plant and fruit detection.
- Growth prediction using accumulated temperature and environmental data.
- Farm-level monitoring and visual analytics.
- Mobile-friendly farmer dashboard.
- Notifications for plant health risks and important growth milestones.

## ⚠️ Disclaimer

The accuracy of image-based growth-stage classification and plant-health assessment depends on the availability and performance of trained models. Weather-based risk information is indicative and does not confirm the presence of a disease.

## 👨‍🌾 Project Purpose

To support smarter, more accessible, and data-driven tomato farming through computer vision, deep learning, weather monitoring, and growth prediction.

