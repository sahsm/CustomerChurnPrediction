# Customer Churn Prediction

## Project Overview

This project develops a machine learning model to predict customer churn for **Interconnect**, a telecommunications company.

The objective is to identify customers who are most likely to cancel their services, allowing the company to implement targeted retention strategies and reduce customer attrition.

Several machine learning models were evaluated, including Logistic Regression, Random Forest, and Gradient Boosting. After hyperparameter tuning, the optimized Gradient Boosting model achieved the best overall predictive performance and was selected as the final model.

---

## Business Problem

Customer churn represents a significant challenge for telecommunications companies. Losing customers increases acquisition costs and reduces long-term revenue.

The goal of this project is to predict which customers are at the highest risk of churn so the company can proactively implement customer retention strategies.

---

## Dataset

The project uses four datasets containing customer information:

- Contract information
- Personal information
- Internet services
- Phone services

These datasets were merged using `customerID` to create a unified dataset for analysis and model training.

---

## Project Workflow

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preparation
- Model Training
- Hyperparameter Tuning
- Model Evaluation
- Feature Importance Analysis

---

## Machine Learning Models

The following models were evaluated:

- DummyClassifier (Baseline)
- Logistic Regression
- Random Forest
- Gradient Boosting

The final model was optimized using GridSearchCV with 5-fold cross-validation.

---

## Results

The optimized **Gradient Boosting** model achieved the best overall performance.

Key metrics:

- ROC-AUC: Best overall
- F1-score: ~0.78
- Strong Precision and Recall

---

## Key Findings

The most important predictors of customer churn were:

- TotalCharges
- ContractDuration
- MonthlyCharges
- Contract Type
- Payment Method

These findings suggest that customer tenure, billing information, and subscription characteristics play an important role in predicting churn.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Repository Structure

```text
TelecomCustomerChurn/
│
├── data/
├── images/
├── Customer_Churn_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---
## Dataset

The dataset used in this project was provided as part of the TripleTen Data Science Bootcamp and is not included in this repository.

To run the notebook, place the required CSV files inside the `data/final_provider/` directory.

---

## Author

**Sara Menger**

Data Science Portfolio Project
