# 🚖 Uber Fare Prediction using Machine Learning

This project predicts the fare amount for Uber rides in New York City using various regression models. It includes data preprocessing, feature engineering, EDA, and model training using **Linear Regression**, **Random Forest**, and **XGBoost**.

---

## 📌 Objective
To develop a machine learning regression model that accurately estimates Uber fares based on trip details, including pickup and drop-off coordinates, passenger count, and datetime features.

---

## 📁 Dataset
The dataset is publicly available on Kaggle and contains:
- `pickup_datetime`
- `pickup_longitude`, `pickup_latitude`
- `dropoff_longitude`, `dropoff_latitude`
- `passenger_count`
- `fare_amount` (target variable)


---

## 🛠️ Technologies Used
- Python (Jupyter Notebook)
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Geopy (for distance calculation)

---

## 📊 Data Preprocessing & Feature Engineering

- **Handled missing/null values**
- **Filtered outliers** in fare amounts, latitudes, longitudes, and passenger count
- **Converted datetime** to separate features: hour, day, month, weekday
- **Calculated Haversine distance** between pickup and drop-off locations
- Final feature set includes:
  - `passenger_count`
  - `distance`
  - `hour`, `day`, `month`, `weekday`

---

## 📈 Exploratory Data Analysis (EDA)

- Distribution plots of fare amount and passenger count
- Correlation heatmap of numerical features
- Visualizations for feature relationships

---

## 🤖 Machine Learning Models Used

| Model              | Description                                 |
|-------------------|---------------------------------------------|
| Linear Regression | Baseline model                              |
| Random Forest     | Tree-based ensemble learning                |
| XGBoost           | Boosted decision tree algorithm for accuracy|

---

## ✅ Evaluation Metrics

- **Root Mean Squared Error (RMSE)**
- **R² Score**

> 🏆 Best Performance:  
> - **Model:** XGBoost  
> - **RMSE:** ~4.12  
> - **R² Score:** ~0.85

---

## 🧠 Key Insights
- **Distance** and **time of day** have strong effects on fare amount
- XGBoost significantly outperformed other models
- Proper feature engineering (e.g., Haversine distance, time features) improved model performance

---

## 🧰 Project Structure
```

Uber-Fare-Prediction/
├── data/                        # Dataset CSV (optional)
├── uber-fare-prediction.ipynb  # Jupyter notebook with code
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies

````

---

## 🚀 How to Run
1. Clone the repository
2. Install dependencies  
   ```bash
   pip install -r requirements.txt
````

3. Open the notebook

   ```bash
   jupyter notebook uber-fare-prediction.ipynb
   ```

---

## 🔮 Future Improvements

* Add live traffic and weather features
* Create an interactive web app using Streamlit/Flask
* Use hyperparameter tuning (GridSearchCV or Optuna)



