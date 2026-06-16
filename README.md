# Medical Insurance Cost Prediction

## Overview

This project applies Machine Learning regression techniques to predict individual medical insurance costs based on demographic and lifestyle factors.

Accurate cost prediction can help insurance companies better estimate risk, improve pricing strategies, and support data-driven decision-making.

The project explores multiple modeling approaches and optimization techniques to evaluate whether predictive performance can be improved beyond a baseline Linear Regression model.

---

## Business Problem

Medical insurance providers need reliable estimates of future healthcare costs in order to:

- Assess customer risk profiles.
- Improve premium pricing strategies.
- Forecast potential expenses.
- Optimize resource allocation.
- Support data-driven underwriting decisions.

This project demonstrates how Machine Learning can be used to model and predict insurance charges using customer-related attributes.

---

## Dataset

The project uses a medical insurance dataset containing demographic and health-related information.

Examples of features include:

- Age
- Sex
- Body Mass Index (BMI)
- Number of children
- Smoking status
- Geographic region

### Target Variable

- **Charges** → Annual medical insurance cost.

---

## Methodology

### 1. Exploratory Data Analysis (EDA)

The dataset was explored to understand:

- Distribution of insurance costs.
- Relationships between variables.
- Impact of smoking habits on medical expenses.
- Potential outliers and data quality issues.

### 2. Data Preparation

Data preprocessing included:

- Categorical feature encoding.
- Train/Test split.
- Feature scaling.
- Dataset transformation and preparation for modeling.

### 3. Baseline Linear Regression Model

A Linear Regression model was trained as the initial benchmark.

The objective was to evaluate how well a simple regression approach could explain variations in insurance costs.

### 4. Model Optimization

Several optimization strategies were explored:

- Feature selection.
- Feature scaling.
- Logarithmic transformation of the target variable.
- Ridge Regression regularization.

### 5. Model Comparison

Different approaches were compared to determine whether additional complexity improved predictive performance.

The results showed that the baseline model already provided strong predictive capabilities and that more complex transformations produced only marginal improvements.

---

## Results

The project demonstrated that Linear Regression can effectively model medical insurance costs using a relatively small set of demographic and lifestyle variables.

Several optimization techniques were tested, including Ridge Regression and logarithmic transformations, but none significantly outperformed the baseline model.

### Key Insight

One of the strongest predictors of insurance costs was smoking status, highlighting the significant impact of lifestyle factors on healthcare expenses.

The analysis also showed that simpler models can often provide performance comparable to more complex alternatives while remaining easier to interpret.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Linear Regression
- Ridge Regression

---

## Model Deployment

The predictive model developed in this project was later used as the foundation for an interactive Streamlit application, allowing users to estimate medical insurance costs through a web interface.

This demonstrates the complete journey from data analysis and model development to deployment and user interaction.

---

## Repository Structure

```text
medical-insurance-cost-prediction/
│
├── README.md
│
├── src/
│   └── 02-linear-regression-medical-insurance-cost.ipynb
│
└── raw/
    └── medical_insurance_cost.csv
```

---

## Key Learnings

- End-to-end Machine Learning workflow.
- Regression modeling for cost prediction.
- Feature engineering and preprocessing.
- Linear Regression optimization.
- Ridge Regression regularization.
- Model comparison and evaluation.
- Translating predictive analytics into business value.
- Deploying Machine Learning solutions through Streamlit.

---

## Author

**Anaís Aponte**

Senior Product Owner | Agile Delivery | Data & AI

GitHub: https://github.com/anaisaponte-GitH
