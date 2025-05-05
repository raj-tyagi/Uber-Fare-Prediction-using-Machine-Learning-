# Uber Fare Prediction using Machine Learning 🚖📊

This project focuses on predicting the fare amount of Uber rides in New York City using machine learning models. The goal is to build a regression model that estimates fares based on features such as pickup/drop-off locations, trip distance, and time-related factors.

## 📌 Objective
To develop and compare different machine learning models to accurately predict Uber ride fares using real-world data. This project demonstrates data preprocessing, feature engineering, EDA, and model evaluation.

---

## 📁 Dataset
The dataset used is publicly available and includes:
- Pickup and drop-off datetime
- Pickup and drop-off coordinates (latitude, longitude)
- Passenger count
- Fare amount (target variable)

> Dataset Source: [Kaggle - Uber Fare Prediction](https://www.kaggle.com/datasets/yasserh/uber-fare-prediction-data)

---

## 🔧 Technologies Used
- **Python**
- **Pandas, NumPy** – Data Manipulation
- **Matplotlib, Seaborn** – Data Visualization
- **Scikit-learn** – ML Models & Evaluation
- **XGBoost** – Gradient Boosted Trees
- **Jupyter Notebook**

---

## 🧹 Data Preprocessing
- Removed null/missing values
- Filtered out invalid geographic coordinates and outliers
- Extracted features from datetime (hour, day, month)
- Calculated haversine distance between pickup and drop-off points

---

## 📊 Exploratory Data Analysis
- Analyzed distributions of fare amount, passenger count, and trip distance
- Visualized pickup locations using scatter plots
- Identified correlations between features

---

## 🤖 Models Implemented
| Model              | Description                                |
|-------------------|--------------------------------------------|
| Linear Regression | Baseline model                             |
| Random Forest     | Ensemble tree-based model                  |
| XGBoost           | Gradient boosting for improved accuracy    |

---

## ✅ Evaluation Metrics
- **Root Mean Squared Error (RMSE)**
- **R² Score (Coefficient of Determination)**

XGBoost performed best, with a significant improvement in prediction accuracy over baseline models.

---

## 📌 Key Learnings
- Real-world datasets require thorough preprocessing and cleaning
- Feature engineering significantly impacts model performance
- Gradient boosting models (XGBoost) outperform simpler regressors for this use case

---

## 📎 Results Snapshot
- Best RMSE: *~3.95 USD*
- Best R² Score: *~0.85* (XGBoost)
- Strong correlation found between distance, time of day, and fare

---

## 🧠 Future Work
- Incorporate weather or traffic data
- Use geospatial clustering for region-based features
- Deploy model with a Flask API for real-time predictions

---

## 📂 Project Structure
```

Uber-Fare-Prediction/
├── data/
├── notebooks/
├── src/
├── visuals/
├── README.md
└── requirements.txt

```



