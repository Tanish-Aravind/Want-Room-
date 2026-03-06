# 🏠 WantRoom 

**WantRoom** is a machine learning powered backend service that predicts **hostel block and room type allocation probabilities based on student rank and historical hostel allotment trends.**

The system analyzes past allotment patterns and generates predictions for students to estimate their chances of getting specific hostel blocks or room types.

This backend exposes REST APIs for prediction, trend analysis, and availability insights.

---

# 🚀 Features

## 📊 Rank-Based Hostel Prediction
Predict probable hostel **block and room type** for a student based on:

- Student rank  
- Year  
- Preferred room type  
- Optional friend rank (for group allotment behavior)

---

## 📁 Batch Prediction
Upload a CSV file containing multiple student entries and receive predictions for all students.

Useful for:

- hostel planning
- analyzing cutoff patterns
- group predictions

---

## 📈 Trend Analytics
View historical hostel trends including:

- AC vs Non-AC ratios
- enrollment numbers
- demand trends across years

---

## 🏢 Availability Insights
Get summarized information about:

- hostel blocks
- room types
- room capacity

---

## ⚙️ Health Monitoring
Check if the API server and machine learning models are running correctly.

---

# 🧠 Machine Learning Model

The prediction system uses tree-based ensemble models:

- **XGBoost**
- **Random Forest**

These models work well because:

- hostel allotment follows **non-linear rank cutoffs**
- decision trees naturally capture **rank thresholds**
- they handle **categorical features and noisy data** effectively

---

# 🏗️ Tech Stack

| Component | Technology |
|-----------|-----------|
| Backend Framework | FastAPI |
| Machine Learning | XGBoost / Random Forest |
| Database | SQLite |
| Data Processing | Pandas / NumPy |
| API Docs | FastAPI Swagger |
