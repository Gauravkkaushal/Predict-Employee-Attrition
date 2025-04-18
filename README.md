# Employee Attrition Prediction

This project creates a machine learning classification model that is used to forecast whether an employee is about to leave a company or not. The model utilizes different features, including job satisfaction, compensation, work climate, and experience, to make precise predictions.

# Project Overview

Employee turnover is a problematic issue for most organizations. By forecasting which employees are likely to leave, companies can take early steps towards enhanced retention. In this project, a **Random Forest Classifier** in a **scikit-learn pipeline** is combined with preprocessing utilities to deal with numerical and categorical data.

# Model Details

- **Model Used**: RandomForestClassifier (scikit-learn)
- **Preprocessing**:
  - Numeric features scaled using `StandardScaler`
- Categorical features encoded with `OneHotEncoder`
  - Combined with `ColumnTransformer`
- **Pipeline**:
  - All preprocessing and modeling steps are encapsulated in a single `Pipeline` for clean and consistent workflow
- **Evaluation Metric**: Classification Report (Precision, Recall, F1-score)

## ⚙️ How It Works

1. CSV file is uploaded and loaded into a Pandas DataFrame
2. Features and target label (`Attrition`) are split
3. Data is divided into training and test sets (80/20)
4. Features are preprocessed:
- Numeric columns are standardized
- Categorical columns are one-hot encoded
5. A `RandomForestClassifier` is fitted on the preprocessed data
6. Model performance is scored on the test set

# Example Features

- JobSatisfaction
- MonthlyIncome (Salary)
- WorkEnvironment
- YearsAtCompany

> **Note**: Feature names may differ with the dataset received.



