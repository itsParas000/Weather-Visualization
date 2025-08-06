# 🌦️ Weather Data Visualization & ML Project

This project focuses on analyzing and modeling historical weather data using Python libraries like pandas, matplotlib, seaborn, and scikit-learn. The dataset used is `WeatherDataset.csv`, containing weather metrics such as temperature, humidity, wind speed, and more.

---

## 📌 Project Goals

- Explore temperature trends over time
- Analyze humidity, wind speed, and visibility patterns
- Visualize relationships between weather variables
- Build predictive ML models (Regression & Classification)

---

## 🛠️ Tools & Libraries

- Python (pandas, numpy)
- matplotlib, seaborn
- scikit-learn (for ML)
- Jupyter Notebook

---

## 📊 Visualizations Included

---
- Temperature trends over time
![Temperature trends over time](Figs/Temperature%20Over%20Time.png)
---

---
- Temperature distribution (histogram)
![Temperature distribution](Figs/Temperature%20Distribution.png)
---

---
- Humidity vs. Temperature scatter plot
![Humidity vs. Temperature scatter plot](Figs/Himidity%20VS%20Temperature.png)
---

---
- Monthly average temperature
![Monthly average temperature](Figs/Average%20Monthly%20Temperature.png)
---

---
- Wind speed distribution
![Wind speed distribution](Figs/Wind%20Speed%20Distribution.png)
---

---
- Weather condition frequency
![Weather condition frequency](Figs/Weather%20Condition%20Count.png)
---

---
- Temperature by precipitation type
![Temperature by precipitation type](Figs/Temperature%20By%20Precipitation%20Type.png)
---

---
- Correlation heatmap
![Correlation heatmap](Figs/Correlation%20Heatmap.png)
---


---

## 🔍 Key Insights

- **Seasonal Pattern**: Clear summer peaks (~30–40°C) and winter lows (~−10°C) across years.
- **Temp Distribution**: Most temps fall between 0°C and 20°C.
- **Humidity**: Strong negative correlation with temperature (−0.63).
- **Visibility**: Moderately positively correlated with temperature (+0.39).
- **Monthly Trends**: July & August are warmest; January & December coldest.
- **Wind**: Most wind speeds range 5–15 km/h.
- **Weather Types**: Cloudy conditions are most common.
- **Rain vs Snow**: Rain occurs at higher temps, snow at freezing levels.

---

## 🤖 Added Machine Learning

### 1. 🔢 Regression – Predicting Temperature

- **Model**: Linear Regression → then improved using Random Forest Regressor

---
- LinearRegression Model
![Actual vs Predicted Temperature](Figs/Actual%20vs%20Predicted%20Temperature%20(LR).png)
---


---
- RandomForestRegressor Model
![RandomForestRegressor Model](Figs/Actual%20vs%20Predicted%20Temperature%20(RFR).png)
---


- **Features Used**: Humidity, Wind Speed, Visibility, Pressure
- **Best Result**: R² Score = 0.65, MSE = 32.19 (Random Forest)
- **Insights**: Model predicts temperature reasonably well. Errors are higher at temperature extremes.

### 2. 🧠 Classification – Predicting Weather Condition

- **Target**: Weather Summary (top 5 classes only)
- **Model**: Random Forest Classifier
- **Accuracy**: 49%
- **Best Predictions**: ‘Foggy’, ‘Partly Cloudy’
- **Challenges**: Some weather types (like ‘Clear’) are harder to classify using basic features.


---
- Confusion Matrix
![Confusion Matrix](Figs/Confusion%20Matrix.png)
---


### 🔚 Conclusion

This project combines Exploratory Data Analysis (EDA) with two supervised ML tasks:
- Regression to predict temperature
- Classification to predict weather conditions

The models are functional but could be improved with more advanced features and tuning.

---

## 📁 Dataset

- File used: `weatherHistory.csv`
- Source: [Kaggle](https://www.kaggle.com)
