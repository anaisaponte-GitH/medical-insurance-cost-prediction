# Medical Insurance Cost Prediction

## Overview

This project applies Machine Learning regression techniques to predict individual medical insurance costs based on demographic and lifestyle factors.

Beyond building a predictive model, the project focuses on understanding the impact of different variables on healthcare expenses and evaluating whether more advanced optimization techniques provide meaningful improvements over a baseline Linear Regression model.

---

## Business Problem

Medical insurance providers need reliable estimates of future healthcare costs to:

- Assess customer risk profiles.
- Improve premium pricing strategies.
- Forecast potential expenses.
- Support data-driven underwriting decisions.

This project demonstrates how Machine Learning can be used to model insurance charges using customer-related attributes.

---

## Dataset

The project uses a medical insurance dataset containing demographic and health-related information.

### Features

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

- Duplicate validation.
- Categorical feature encoding.
- Train/Test split.
- Feature scaling experiments.
- Dataset preparation for modeling.

### 3. Baseline Model

A Linear Regression model was trained as the initial benchmark.

The objective was to evaluate how effectively a simple regression approach could explain variations in insurance costs.

### 4. Model Optimization

Several optimization strategies were evaluated:

- Feature removal.
- Feature scaling.
- Logarithmic transformation of the target variable.
- Lasso Regression.
- Ridge Regression.

### 5. Model Comparison

Different approaches were compared to determine whether additional complexity improved predictive performance.

---

## Model Evaluation

### Performance Comparison (R² Score)

| Model | R² Score |
|---------|---------:|
| Original Linear Regression | 0.81 |
| Without Sex Feature | 0.81 |
| Scaled Model | 0.81 |
| Lasso (Log + Scaled) | 0.67 |
| Linear Regression (Log) | 0.71 |
| Ridge (Log + Scaled) | 0.72 |

### Final Model Selection

After evaluating multiple optimization strategies, the original Linear Regression model was selected as the final solution.

Although feature scaling, logarithmic transformations and regularization techniques were explored, none provided a meaningful improvement over the baseline model when evaluated in the original business scale.

The final model offered the best balance between:

- Predictive performance
- Simplicity
- Interpretability
- Business usability

---

## Key Findings

- Smoking status was the strongest predictor of insurance costs.
- Age and BMI showed a significant relationship with healthcare expenses.
- The baseline Linear Regression model already achieved strong predictive performance.
- More complex transformations introduced additional complexity without delivering substantial business value.
- Simpler and interpretable models can often outperform more sophisticated alternatives in real-world scenarios.

---

## Results

The project demonstrated that Linear Regression can effectively model medical insurance costs using a relatively small set of demographic and lifestyle variables.

A key insight from the analysis was that optimization techniques should not be adopted solely because they are more advanced. Their value must be justified through measurable improvements in predictive performance and business outcomes.

---

## Model Deployment

The selected model was exported as a `.sav` file and later used as the foundation for an interactive Streamlit application that allows users to estimate medical insurance costs through a web interface.

This project therefore covers the complete Machine Learning workflow:

- Data exploration
- Feature engineering
- Model training
- Model evaluation
- Model selection
- Model deployment

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
- Lasso Regression
- Joblib
- Jupyter Notebook

---

## Repository Structure

```text
medical-insurance-cost-prediction/
│
├── README.md
│
├── raw/
│   └── medical_insurance_cost.csv
│
└── src/
    └── 02-linear-regression-medical-insurance-cost.ipynb
```

---

## Key Learnings

- End-to-end Machine Learning workflow.
- Regression modeling for cost prediction.
- Feature engineering and preprocessing.
- Model evaluation and comparison.
- Business-oriented model selection.
- Translating predictive analytics into actionable insights.
- Preparing models for deployment in production environments.

---

## Author

**Anaís Aponte**

Senior Product Owner | Agile Delivery | Data & AI

GitHub: https://github.com/anaisaponte-GitH

LinkedIn: https://linkedin.com/in/anaisaponte
