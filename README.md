# Diabetes Patient Outcome Prediction: Model Development and Tuning

**Authors**: Benoit Schiermeier, Ava Wagner, Jason Reed, Julianne Conlee

**Dataset**: [UCI Diabetes Dataset (130 US Hospitals, 1999–2008)](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

---

## Overview
This project applies data science and machine learning to predict diabetes status (healthy, prediabetic, diabetic) based on clinical indicators. Our work focuses on cleaning the data, performing exploratory analysis, selecting significant features, and building predictive models.

---

## Project Steps

### Data Preparation
- Loaded and cleaned dataset (handled missing values, dropped duplicates).
- Corrected datatypes and standardized continuous features (e.g., BMI, Age).

### Exploratory Data Analysis (EDA)
- Correlation heatmaps to identify influential features.
- Distribution analysis of Age, BMI, General Health, and Income.
- Analysis of education level, sex, blood pressure, and cholesterol impacts on diabetes status.

### Statistical Significance Testing
- t-tests and chi-squared tests for feature selection.
- Confirmed significant predictors: BMI, Age, High Blood Pressure, High Cholesterol, General Health, and Physical Health.

### Feature Engineering
- Created BMI categories (Normal, Overweight, Obese) for additional analysis.

### Model Building and Evaluation
- Models Trained: Support Vector Machine (SVM), Random Forest (RF), and K-Nearest Neighbors (KNN).
- GridSearchCV used for hyperparameter tuning.
- StandardScaler applied to continuous variables.
- Evaluated models using accuracy, precision, recall, and F1-score.

### Bias and Fairness Analysis
- Detected gender and income bias in predictions.
- Highlighted model limitations due to sample imbalances.

---

## Key Results
- **Best Test Accuracy**: Random Forest — 83.0%
- **Significant Bias Observed**: Model overpredicts diabetes in males and lower-income groups.
- **Top Predictive Features**: General Health, BMI, Age, Blood Pressure, Cholesterol.

---

## Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Scipy)
- Jupyter Notebook

---

## Potential Impacts
This model can help identify patients at higher risk for diabetes earlier, improving preventative healthcare efforts. However, future work should address biases in gender and income prediction to ensure equitable model performance.

