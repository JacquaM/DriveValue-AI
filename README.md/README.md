#  DriveValue AI

**Author:** Jacqualine Makgolana

---

# Project Overview

## Explainable Machine Learning Framework for Used Vehicle Price Prediction

An end-to-end machine learning project that predicts used vehicle asking prices using Random Forest Regression and Explainable AI (SHAP), following the CRISP-DM methodology.
---

# Business Problem

Used vehicle pricing is often subjective, inconsistent, and influenced by human judgement.

DriveValue AI provides a data-driven pricing framework capable of generating fair and consistent asking price estimates while reducing pricing bias.

The solution is designed to support:

- Vehicle dealerships
- Online vehicle marketplaces
- Financial institutions
- Private vehicle sellers

---

# Business Objectives

- Predict used vehicle asking prices using machine learning.
- Compare multiple regression algorithms.
- Identify the best-performing predictive model.
- Improve model transparency using Explainable AI.
- Demonstrate deployment readiness.

---

# Dataset

The project uses a real-world dataset containing used vehicle listings.

**Dataset Summary**

- **Records:** 14,988 vehicle listings
- **Features:** 466 engineered features
- **Target Variable:** Asking Price (₹)

---

# CRISP-DM Methodology

The project follows the CRISP-DM framework.

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modelling
5. Evaluation
6. Deployment

---

# Repository Structure

```text
DRIVEVALUE_AI/

├── app/
│   └── app.py
│
├── Data/
│   ├── raw/
│   └── processed/
│
├── images/
│
├── models/
│   ├── random_forest_model.pkl
│   ├── feature_columns.pkl
│   ├── model_columns.pkl
│   └── categories.pkl
│
├── notebooks/
│   ├── 01_Data_Audit.ipynb
│   ├── 02_Exploratory_Data_Analysis.ipynb
│   ├── 03_Feature_Engineering.ipynb
│   ├── 04_Model_Building.ipynb
│   ├── 05_Model_Optimization_and_Explainability.ipynb
│   └── 06_Final_Evaluation_Deployment.ipynb
│
├── reports/
│   ├── Executive_Summary.pdf
│   └── Final_Project_Report.pdf
│
├── src/
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Machine Learning Models

The following regression algorithms were evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

After evaluation, the **Random Forest Regressor** achieved the strongest predictive performance and was selected as the final production model.

---

# Model Performance

| Metric | Value |
|---------|-------|
| MAE | ₹398,156 |
| RMSE | ₹1,267,201 |
| R² Score | 0.446 |

---

# Explainable AI

Model transparency was achieved using **SHAP (SHapley Additive Explanations).**

SHAP was used to:

- Explain feature importance
- Interpret prediction behaviour
- Increase stakeholder trust
- Support transparent pricing decisions

# Streamlit Application

DriveValue AI includes an interactive Streamlit application that enables users to estimate used vehicle asking prices by entering:

- Vehicle Year
- Mileage
- Brand
- Model
- Fuel Type
- Transmission
- Ownership History
- Listing Date

The application loads the trained Random Forest model and generates real-time price predictions.
---

# Deployment Workflow

Customer Vehicle Details

↓

Data Validation

↓

Feature Engineering

↓

Random Forest Model

↓

SHAP Explainability

↓

Predicted Vehicle Price

↓

Dealer Dashboard

---

# Key Findings

- Vehicle age strongly influences asking price.
- Vehicle brand significantly affects predicted value.
- Vehicle model contributes additional pricing information.
- Mileage remains an important pricing factor.
- Random Forest produced the highest predictive accuracy.
- SHAP successfully improved model interpretability.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Random Forest Regression
- SHAP
- Plotly
- Matplotlib
- Joblib
- Streamlit
- Jupyter Notebook
---

# Future Improvements

- Deploy the application to Streamlit Community Cloud or Azure.
- Integrate live vehicle marketplace data.
- Automate periodic model retraining.
- Improve prediction accuracy using Gradient Boosting or XGBoost.
- Build an interactive dealer analytics dashboard..

---

# Installation

Clone the repository

```bash
git clone https://github.com/JacquaM/DriveValue-AI.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```
# Run the Streamlit Application

```bash
cd app
streamlit run App/app.py

---

# Author

**Jacqualine Makgolana**

Data Science Capstone Project

DriveValue AI — 2026
## License

This project was developed for academic purposes as part of the ZAIO Data Science Capstone Project.