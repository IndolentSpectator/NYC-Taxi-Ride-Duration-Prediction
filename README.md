# NYC-Taxi-Ride-Duration-Prediction
# 🚖 NYC Taxi Ride Duration Prediction: Automatidata Project

## 📌 Project Overview

This project leverages **machine learning** to predict the duration of taxi rides in **New York City** using **historical trip data**. By analyzing key features such as pickup/drop-off locations, time of day, and weather conditions, we aim to enhance route optimization for drivers and provide **accurate ride-time estimates** to passengers.

---

## 📝 Business Understanding

### 🎯 Business Need and Objective

NYC taxi drivers and passengers often face unpredictable ride durations due to **traffic congestion, weather conditions, and time-of-day variations**. The objective of this project is to:

- **Accurately predict ride duration** to help drivers plan routes efficiently.
- **Provide passengers with estimated trip times** to improve customer satisfaction.
- **Optimize fleet management for taxi companies** using predictive insights.

### 🚕 Stakeholders

- **Taxi Drivers**: To optimize routes and manage time better.
- **Passengers**: To receive reliable ETAs and reduce uncertainty.
- **Fleet Operators & Regulators**: To analyze taxi demand patterns and improve urban mobility.

---

## 🗂️ Data Understanding & Feature Engineering

### 📂 Dataset

- **Source**: NYC Yellow Taxi Trip Data (2017)
- **Additional Data**: NYC weather and traffic conditions
- **Attributes**:
  - `pickup_datetime` (timestamp)
  - `dropoff_datetime` (timestamp)
  - `trip_distance` (miles)
  - `pickup_longitude`, `pickup_latitude` (GPS coordinates)
  - `dropoff_longitude`, `dropoff_latitude` (GPS coordinates)
  - `passenger_count`
  - `fare_amount`

### 🔎 Feature Engineering

- **Time-based Features**: Hour of the day, weekday vs. weekend analysis.
- **Distance Calculation**: Haversine distance between pickup and drop-off points.
- **Weather Conditions**: Rain, snow, temperature (if available).
- **Traffic Indicators**: Peak vs. off-peak hours based on NYC traffic patterns.

---

## 🏗️ Modeling & Evaluation

### 🤖 Machine Learning Models Used

1. **Linear Regression** (Baseline model)
2. **Random Forest Regressor** (Improved predictive accuracy)
3. **Gradient Boosting (XGBoost, LightGBM)** (Fine-tuned ensemble models)
4. **Neural Networks** (Exploring deep learning for time-series patterns)

### 📊 Evaluation Metrics

- **Mean Absolute Error (MAE)** – Measures average prediction error.
- **Root Mean Squared Error (RMSE)** – Penalizes larger errors more than MAE.
- **R² Score** – Indicates how well the model explains variance in trip duration.

---

## ⚖️ Ethical Considerations

### 🚨 Key Issues

- **Bias in Data**: Models may not generalize well to all neighborhoods.
- **Data Privacy**: Ensuring anonymized trip details while maintaining accuracy.
- **Fairness**: Avoiding model bias against underserved areas.

The project aims to:

- **Ensure fair representation of all boroughs**.
- **Mitigate bias in ride duration predictions**.
- **Maintain transparent AI model deployment**.

---

## 🏆 Conclusion & Recommendations

### ✅ Key Findings

- **Traffic congestion, weather, and pickup/drop-off locations** are major factors influencing ride duration.
- **Haversine distance is a strong predictor**, but additional factors like **road conditions** and **driver behavior** could improve accuracy.

### 🚀 Next Steps

- **Integrate real-time weather API** for improved predictions.
- **Enhance models with traffic congestion data** for better route optimization.
- **Deploy model via an API** for real-time trip estimation.

---

## 🙌 Acknowledgments

- **Libraries Used**: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn.

---

