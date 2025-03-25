# World Bank Projects Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-1.6.0-green.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-orange.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.4.0-red.svg)
![F1 Score](https://img.shields.io/badge/F1_Score-71.7%25-brightgreen.svg)

## 📊 Project Overview

This repository contains a comprehensive analysis of World Bank project data, focusing on predicting project outcomes using machine learning techniques. The analysis uses XGBoost classification to identify key factors that influence whether development projects will be successfully completed or dropped.

## 🎯 Key Objectives

- Predict World Bank project outcomes (Closed vs. Dropped) with high precision and recall
- Identify the most influential factors determining project success
- Develop a robust model that handles class imbalance and missing data
- Provide actionable insights for better project planning and risk assessment

## 📋 Dataset

The dataset contains information about World Bank project lending across 27 features:

- **Basic Info**: Project ID, region, country, status, name, and URL
- **Financial Data**: Project cost, IBRD/IDA commitments, grant amounts
- **Timeline**: Board approval date, closing date
- **Classifications**: Environmental assessment codes, risk ratings
- **Sectors & Themes**: Primary sectors and thematic focuses

## 🔍 Exploratory Data Analysis

The exploratory analysis revealed several key insights:

- The dataset is significantly imbalanced (90% closed, 10% dropped projects)
- High missing data rates in certain fields (30%+ in key variables)
- Regional and financial type variations in project outcomes
- Distinct patterns in environmental assessment categories

## 🧮 Methodology

1. **Data Preprocessing**:
   - Handling of missing values and data type conversions
   - Feature selection and engineering
   - Addressing class imbalance

2. **Model Development**:
   - XGBoost classification with optimized hyperparameters
   - RandomizedSearchCV for parameter tuning
   - Evaluation metrics prioritizing F1 score due to class imbalance

3. **Model Evaluation**:
   - Confusion matrix analysis
   - Precision (80.6%) and Recall (64.6%) assessment
   - Error metrics (MAE, MSE, RMSE)

## 📈 Results

The optimized XGBoost model achieved:
- **F1 Score**: 71.7%
- **Precision**: 80.6%
- **Recall**: 64.6%
- **Accuracy**: 94.6%
- **RMSE**: 0.233


## 💻 Setup and Installation

```bash
# Clone this repository
git clone https://github.com/faseehahmed26/World-Bank-Projects.git

# Navigate to the project directory
cd World-Bank-Projects

# Install dependencies
pip install -r requirements.txt

# Run the notebooks
jupyter notebook
🔮 Future Work

Implement more sophisticated handling of missing data
Explore deep learning approaches for improved accuracy
Develop interactive visualization dashboards
Incorporate additional external datasets for enhanced predictions

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.


