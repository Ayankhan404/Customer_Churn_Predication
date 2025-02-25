# Customer Churn Prediction Model

## Overview

This project focuses on building an end-to-end machine learning pipeline to predict customer churn. The dataset contains various customer attributes, including demographic information, service usage, and account details. The goal is to analyze the dataset, preprocess the data, perform exploratory data analysis (EDA), build a machine learning model, and evaluate its performance to identify customers likely to churn.

## Technologies Used

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn, XGBoost, Pickle

## Project Workflow

### 1. Data Import and Understanding

- Import necessary libraries (Pandas, NumPy, Matplotlib, Seaborn).
- Load the dataset and inspect the structure of the data.
- Identify column names and data types.

### 2. Data Preprocessing

- Check for missing values using a heatmap.
- Found missing values in the `TotalCharges` column and replaced them with `0.0`.
- Identified incorrect data types and corrected them.
- Dropped unused columns.
- Separated numerical and categorical features.
- Printed unique values of each column.

### 3. Handling Imbalanced Data

- Found that the `Churn` column (target variable) is imbalanced.
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to handle imbalance.

### 4. Exploratory Data Analysis (EDA)

- Used the `describe()` method to understand numerical columns.
- **Univariate Analysis**:
  - Plotted boxplots for numerical columns.
  - Checked for outliers (found none).
  - Plotted count plots for categorical features.
- Converted the categorical target column (`Churn`) into numerical values.
- Applied **Label Encoding** on categorical features and saved the encoding using **Pickle** for future use.

### 5. Model Building and Selection

- Split the dataset into **training (train)** and **testing (test)** sets.
- Tried different machine learning models:
  - **XGBClassifier**
  - **RandomForestClassifier**
  - **DecisionTreeClassifier**
- Used **cross-validation** and **confusion matrix** to evaluate models.
- **XGBoost performed the best** with the highest accuracy and precision.

## How to Run the Project

### Prerequisites

Ensure you have the following dependencies installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost pickle-mixin
```

### Steps to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction
```

2. Use the saved model to make predictions on new customer data.

## Results
- **XGBoost Model** achieved the best performance.
- The model can now be used to predict if a customer is likely to churn, allowing businesses to take proactive measures.

## Future Enhancements
- **Hyperparameter tuning** for further model optimization.
- **Deploying the model** using Flask or FastAPI.
- **Feature engineering** to improve predictive performance.

## Conclusion
This project successfully demonstrates how to build a customer churn prediction system from data preprocessing to model selection. The final model can help businesses reduce churn and improve customer retention.

---
### Author
**Ayan Khan**

Feel free to contribute or provide suggestions! 🚀


## Connect with Me

[LinkedIn](https://www.linkedin.com/in/ayan-khan-917611250/)
```
