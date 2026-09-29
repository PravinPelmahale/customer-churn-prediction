# Customer Churn Prediction

A machine learning project that predicts whether a telecom customer is likely to churn using Logistic Regression.

## Objective

The objective of this project is to build a classification model that predicts customer churn based on customer demographics, services, contract details, and billing information.

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains information about:
- Customer demographics
- Services used
- Contract type
- Payment method
- Tenure
- Monthly charges
- Total charges

Target variable:
- `Churn = 1` → Customer churned
- `Churn = 0` → Customer did not churn

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Workflow

1. Data loading
2. Data cleaning
3. Exploratory Data Analysis (EDA)
4. Handling missing values
5. Feature engineering
6. Categorical feature encoding
7. Train-test split
8. Feature scaling
9. Handling class imbalance
10. Logistic Regression model training
11. Model evaluation

## Model

### Logistic Regression

Logistic Regression was used as the classification algorithm to predict whether a customer will churn.

Class imbalance was handled using:

```python
LogisticRegression(
    class_weight='balanced',
    max_iter=1000,
    random_state=42
)

Evaluation Metrics
The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC-AUC
- PR-AUC
Results
The final Logistic Regression model achieved approximately:
- Accuracy: 73.8%
- Precision: 50.4%
- Recall: 78.3%
- F1-score: 61.4%
- ROC-AUC: 0.84
- PR-AUC: 0.63

The model achieved relatively high recall for churn customers, meaning it was able to identify a large proportion of customers who actually churned.

Key Learning

This project helped demonstrate the complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, categorical encoding, feature scaling, handling class imbalance, model training, and evaluation.

Project Structure

customer-churn-prediction/
│
├── Telco_Customer_Churn.ipynb
├── README.md
└── requirements.txt

