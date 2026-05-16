# 🫀 Cardiovascular Disease Risk Prediction & Machine Learning Analysis

## 📌 1. Project Title
**Epidemiological Risk Stratification and Machine Learning Classification of Cardiovascular Disease Using Clinical Biomarkers.**

Author - Phyo Nyein Chan
---

## 🔍 2. Background & Objectives
Cardiovascular diseases (CVDs) are complex and influenced by a combination of demographic, lifestyle, and biological mechanisms. 
The core objectives of this project are:
- To analyze **sex-specific differences** in heart disease prevalence and presentation.
- To quantify the impact of risk factors like age, resting blood pressure, and cholesterol.
- To evaluate clinical feature importance using artificial intelligence to contribute towards improved risk stratification and prevention strategies.

---

## 📂 3. Dataset Specifications & Source
- **Dataset Name:** UCI Machine Learning Repository — Heart Disease Dataset (Cleveland Cohort)
- **Original Authors:** Andras Janosi, William Steinbrunn, Matthias Pfisterer, and Robert Detrano (1988).
- **Direct Dataset Link:** [UCI Heart Disease Dataset via Kaggle](https://kaggle.com)
- **Data Size:** 297 patient cases analyzed (after filtering out missing diagnostic data from `ca` and `thal` variables).

---

## 🛠️ 4. Methods & Statistical Approaches Used
This project utilizes an interdisciplinary workflow combining traditional biostatistics with medical machine learning:
1. **Data Harmonization:** Handled missing values systematically via the `tidyverse` suite in R.
2. **Descriptive Analytics:** Visualized demographic groupings utilizing `ggplot2` bar distributions.
3. **Traditional Epidemiology Statistics:** Executed **Binary Logistic Regression** via `glm()` to calculate adjusted **Odds Ratios (OR)** and 95% Confidence Intervals.
4. **Model Diagnostics:** Validated assumptions against multicollinearity using the **Variance Inflation Factor (VIF)** via the `car` library.
5. **Advanced Machine Learning:** Implemented a **Random Forest Classification Algorithm** via `randomForest` with an 80/20 train-test split cross-validation.
6. **Performance Metrics Evaluation:** Calculated Sensitivity, Specificity, Balanced Accuracy, and plotted **Receiver Operating Characteristic (ROC-AUC)** curves via `pROC` and `caret`.

---

## 🏆 5. Key Research Findings
- **Significant Sex-Specific Differences:** Binary logistic regression confirmed a major gender disparity; **Male patients exhibit approximately 4.9 times higher odds (OR = 4.90, p < 0.001) of presenting heart disease** compared to female cohorts when controlling for clinical parameters.
- **Primary Diagnostic Predictors:** While age and gender are strong background variables, the Machine Learning algorithm identified **Chest Pain Type (`cp`)** and **Maximum Heart Rate Achieved (`thalach`)** as possessing the highest feature importance for active clinical classification.
- **Robust Model Diagnostics:** The final predictive architecture demonstrated a **Balanced Accuracy of 77.37%**, an exceptional **Sensitivity of 84.38%**, and a discriminatory **ROC-AUC profile of 0.73**, proving its efficacy as a supportive screening layout.

---

## 🔗 6. Live Interactive Report
[👉 CLICK HERE TO VIEW THE FULL INTERACTIVE MEDICAL REPORT](https://phyonyeinchan.github.io/cardiovascular-risk-prediction-r/cardiovascular_analysis.html)
