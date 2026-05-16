# cardiovascular-risk-prediction-r
# Cardiovascular Disease Risk Prediction & Machine Learning Analysis

## 📌 Project Overview
This project focuses on identifying key clinical determinants of cardiovascular disease and building a predictive model using both traditional epidemiology statistics and advanced machine learning. The primary goal is aligned with understanding sex-specific differences, risk stratification, and feature importance in cardiometabolic diseases.

### 🔗 Live Interactive Report
[👉 CLICK HERE TO VIEW THE INTERACTIVE HTML REPORT](https://phyonyeinchan.github.io/cardiovascular-risk-prediction-r/)

---

## 📊 Dataset Specifications
- **Source:** UCI Machine Learning Repository (Cleveland Clinic Foundation)
- **Sample Size:** 297 patients (after removing 6 rows with missing data in `ca` and `thal` columns)
- **Features:** 14 clinical attributes including age, sex, chest pain type (`cp`), resting blood pressure (`trestbps`), cholesterol (`chol`), and maximum heart rate (`thalach`).
- **Target Variable:** Binary classification (0 = No Disease, 1 = Heart Disease Present)

---

## 🛠️ Methodology & Statistical Approaches
This analysis leverages multiple methodologies required in advanced epidemiological research:
1. **Data Cleaning & Descriptive Statistics:** Handled missing values systematically and analyzed sex-specific distributions.
2. **Traditional Epidemiology Modeling:** Conducted Binary Logistic Regression to estimate **Odds Ratios (OR)** with 95% Confidence Intervals.
3. **Model Diagnostics:** Performed Multicollinearity checks using Variance Inflation Factor (VIF).
4. **Machine Learning & Feature Importance:** Implemented a **Random Forest** algorithm to classify patients and rank clinical feature importance.
5. **Performance Evaluation:** Evaluated models using Sensitivity, Specificity, Balanced Accuracy, and ROC-AUC curve analysis.

---

## 📈 Key Findings
- **Sex-Specific Differences:** Logistic regression confirmed that male patients have a significantly higher risk of cardiovascular disease compared to females (p < 0.001).
- **Strongest Predictors:** Both traditional statistics and Machine Learning (Random Forest) identified **chest pain type (`cp`)** and **maximum heart rate achieved (`thalach`)** as the most critical diagnostic markers for predicting heart disease presence.
- **Model Performance:** The predictive model achieved a **Balanced Accuracy of 77.37%** and a **Sensitivity of 84.38%**, proving robust diagnostic capabilities with an **AUC-ROC of 0.73**.

---

## 💻 Tech Stack & Packages Used
- **Language:** R (v4.6.0)
- **Environment:** RStudio / R Markdown
- **Libraries:**
  - `tidyverse` (Data manipulation & ggplot2 visualization)
  - `car` (VIF Diagnostic Test)
  - `pROC` (ROC-AUC Analysis)
  - `caret` & `randomForest` (Machine Learning workflow)

---

## 📂 Repository Structure
- `cardiovascular_analysis.Rmd` — The original executable R Markdown source code.
- `cardiovascular_analysis.html` — The knitted professional output report containing all charts and analytical text.
- `heart_disease_cleveland.csv` — The cleaned dataset used for this study.
