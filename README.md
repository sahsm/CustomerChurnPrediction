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

The dataset was provided as part of the TripleTen Data Science Bootcamp and is not included in this repository.

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

The optimized **Gradient Boosting** model achieved the best overall performance among the evaluated models, with an **F1-score of approximately 0.78**.

The model also demonstrated a strong balance between precision and recall, making it suitable for identifying customers at risk of churn while limiting unnecessary retention interventions.

---

## Key Findings

Feature importance analysis identified the following variables as some of the strongest predictors of churn:

- TotalCharges
- ContractDuration
- MonthlyCharges
- Contract Type
- Payment Method

These results indicate that customer tenure, pricing, contract structure, and payment behavior are important signals of churn risk.

From a business perspective, these factors could help guide retention strategies toward customers displaying higher-risk characteristics.

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

## What I Learned

This project strengthened my understanding of the complete supervised machine learning workflow, particularly:

- Building classification pipelines from multiple data sources
- Handling preprocessing and feature engineering for mixed data types
- Comparing models using metrics beyond accuracy
- Using cross-validation and hyperparameter tuning for model selection
- Evaluating the trade-off between precision and recall in a business context
- Interpreting feature importance and translating model results into actionable business insights

---

## Future Improvements

Potential next steps for this project include:

- Testing additional boosting algorithms such as XGBoost or LightGBM
- Exploring more advanced feature engineering and feature selection techniques
- Evaluating probability thresholds based on the business cost of false positives and false negatives
- Adding model explainability techniques such as SHAP to better understand individual churn predictions
- Developing a simple dashboard or application to make churn-risk predictions more accessible to business users

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

## How to Run

1. Clone this repository.

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Place the required CSV files inside:

```text
data/final_provider/
```

4. Open and run:

```text
Customer_Churn_Prediction.ipynb
```

The original dataset was provided as part of the TripleTen Data Science Bootcamp and is not included in this repository.

---

## Author

**Sara Menger**

Data Science Portfolio Project
