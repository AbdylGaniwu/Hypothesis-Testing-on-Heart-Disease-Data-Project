# Hypothesis Testing on Heart Disease Data

## Project Overview

This project performs **hypothesis testing** on a dataset of heart disease patients, focusing on key health metrics such as **cholesterol levels** and **fasting blood sugar (fbs)**. The goal is to determine if specific health conditions, such as high cholesterol and high blood sugar, are significantly associated with heart disease. This is done using **one-sample t-tests** and **binomial tests**, which form the core of the statistical analysis in this project.

---

## Dataset

The dataset consists of 303 patient records, each containing the following features:
- **Cholesterol levels (chol)**
- **Fasting blood sugar (fbs)**
- **Presence or absence of heart disease**

---

## Key Hypothesis Tests and Findings

### 1. Cholesterol Level Analysis

- **Test 1: Do people with heart disease have an average cholesterol level greater than 240 mg/dL?**
  - **Null Hypothesis (H₀)**: People with heart disease have an average cholesterol level of 240 mg/dL.
  - **Alternative Hypothesis (H₁)**: People with heart disease have an average cholesterol level greater than 240 mg/dL.
  - **Results**:  
    - **Mean Cholesterol Level**: 251.47 mg/dL  
    - **p-value**: 0.0035  
    - **Conclusion**: Since the p-value is much lower than the 0.05 significance threshold, we reject the null hypothesis. This provides strong statistical evidence that people with heart disease have higher-than-average cholesterol levels.

- **Test 2: Do people without heart disease have an average cholesterol level greater than 240 mg/dL?**
  - **Null Hypothesis (H₀)**: People without heart disease have an average cholesterol level of 240 mg/dL.
  - **Alternative Hypothesis (H₁)**: People without heart disease have an average cholesterol level greater than 240 mg/dL.
  - **Results**:  
    - **Mean Cholesterol Level**: 242.64 mg/dL  
    - **p-value**: 0.263  
    - **Conclusion**: The p-value is greater than 0.05, indicating no strong evidence to reject the null hypothesis. We conclude that there is no significant difference in cholesterol levels for people without heart disease compared to 240 mg/dL.

### 2. Fasting Blood Sugar (fbs) Analysis

- **Test 3: Is the proportion of patients with fasting blood sugar > 120 mg/dL significantly higher than the expected 8%?**
  - **Null Hypothesis (H₀)**: The proportion of patients with fasting blood sugar > 120 mg/dL is 8%.
  - **Alternative Hypothesis (H₁)**: The proportion of patients with fasting blood sugar > 120 mg/dL is higher than 8%.
  - **Results**:  
    - **Number of Patients with fbs > 120 mg/dL**: 45 out of 303  
    - **p-value**: 0.0000469  
    - **Conclusion**: Since the p-value is extremely small, we reject the null hypothesis. This suggests that the proportion of patients with high fasting blood sugar is significantly greater than the expected 8%.

---

## Statistical Methods Used

1. **One-Sample T-Test**:  
   - Used to determine if the mean cholesterol level differs significantly from 240 mg/dL.
2. **Binomial Test**:  
   - Used to test if the proportion of patients with high fasting blood sugar differs significantly from an 8% population prevalence.

---

## Files in this Repository

- **heart_disease.csv**: The dataset used for analysis.
- **heart_disease_analysis.py**: Python script containing the full analysis.
- **README.md**: This file, describing the project and the hypothesis testing approach.

---

## Libraries Used

- **Pandas**: For data manipulation.
- **NumPy**: For numerical operations.
- **SciPy**: For statistical hypothesis testing.

---

## Conclusion

This project demonstrates how statistical hypothesis testing can be applied to determine the relationship between health metrics and heart disease. The findings provide valuable insights into the health risks associated with elevated cholesterol and fasting blood sugar levels, which could have important clinical or public health implications.

