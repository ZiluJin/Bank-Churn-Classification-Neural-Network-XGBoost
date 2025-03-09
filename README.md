# Bank Churn Prediction

## Overview
This project aims to predict whether a bank customer will churn, helping financial institution take prebentive actions.
I employ multiple machine learning models (XGBoost, DNN, Random Forest, etc.) and optimize their performance using **hyperparameter tuning (GridSearchCV).**

## Dataset
- Source: Kaggle
- Features
  - `CreditScore` - Customer's credit score
  - `Geography` - Country of the customer
  - `Gender` - Customer's gender
  - `Age` - Customer's age
  - `Balance` - Account balance
  - `NumOfProducts` - Number of banking products purchased
  - `IsActiveMember` - Whether the customer is active
  - `Exited` - **Target variable** (1 = Churned, 0 = Retained)
 
## Technologies Used
- **Data Processing**
  - Handling missing values
  - `LabelEncoder` for categorical encoding (`Gender`, `Geography`)
  - `StandardScaler` for feature normalization (`CreditScore`, `Balance`, `Age`)
  - Feature engineering (Age binning with `pd.cut()`)

- **Machine Learning Models**
  - **GradientBoostClassifier**
  - **DNN (Deep Neural Network)**
  - **XGBClassifier**

- **Hyperparameter Tuning**
  - `GridSearchCV`
  - Cross-validation (`cross_val_score`)

---


## Results & Evaluation
| **Model** | **Accuracy** | **Precision** | **Recall** | **F1-score** |
|------|------|------|------|------|
| GradientBoostClassifier | 86.5% | -- | -- | -- |
| DNN (Deep Neural Network) | 86.5% | -- | -- | -- |
| XGBClassifier | **86.5%** | **86.8%** | **86.8%** | **86.8%** |


