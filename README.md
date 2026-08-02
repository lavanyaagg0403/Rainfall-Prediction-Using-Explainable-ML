# 🌧️ Rainfall Prediction Using Explainable Machine Learning

A machine learning project that predicts daily rainfall using historical weather data from major Indian cities. The project applies data preprocessing, exploratory data analysis (EDA), feature engineering, and Random Forest Regression to analyse rainfall patterns and identify the most influential weather variables through feature importance analysis.

---

## 📌 Project Overview

Rainfall prediction plays an important role in agriculture, water resource management, and disaster preparedness. This project uses a historical weather dataset covering multiple Indian cities from **2000 to 2024** to build a regression model capable of predicting daily rainfall.

The workflow includes:

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Random Forest Regression
- Model evaluation
- Feature importance analysis

---

## 📂 Dataset

**Dataset:** India Daily Weather (2000–2024) – Major Cities

**Source:** Kaggle

**Records:** 91,320 daily observations

**Features include:**

- City
- Maximum & minimum temperature
- Apparent temperature
- Rainfall
- Weather code
- Wind speed
- Wind gusts
- Wind direction
- Date

**Target Variable**

- `rain_sum`

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## 🔄 Project Workflow

1. Data Collection
2. Data Preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Train-Test Split (80:20)
6. Random Forest Regression
7. Model Evaluation
8. Feature Importance Analysis

---

## 📊 Model Performance

| Metric | Value |
|--------|------:|
| MAE | 1.091 |
| RMSE | 3.799 |
| R² Score | 0.820 |

These results indicate that the model explains approximately **82% of the variation** in daily rainfall within the dataset.

---

## 📈 Visualizations

The notebook includes:

- Rainfall Distribution Histogram
- Average Rainfall by City
- Correlation Heatmap
- Actual vs Predicted Scatter Plot
- Feature Importance Plot

---

## 📁 Repository Structure

```text
Rainfall-Prediction-Using-Random-Forest
│
├── README.md
├── Rainfall_Prediction.ipynb
├── requirements.txt
├── .gitignore
├── LICENSE
└── images/
```

---

## 🚀 Future Improvements

- Compare multiple regression models
- Use real-time weather data
- Explore SHAP or LIME for deeper model interpretability
- Develop an interactive dashboard for rainfall prediction

---

## 👩‍💻 Author

**Lavanya Aggarwal**

B.Tech Computer Science Engineering

Amity University Noida

GitHub: https://github.com/lavanyaagg0403

LinkedIn: https://www.linkedin.com/in/lavanya-agg0403/

---

## ⭐ If you found this project useful, consider giving it a star.
