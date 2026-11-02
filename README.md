# Telecom Customer Churn Prediction Using Machine Learning

## Project Overview

This project explores customer churn prediction using the IBM Telco Customer Churn dataset. It uses exploratory data analysis (EDA) and machine learning classification models to identify customers who may discontinue their services.

The project compares four machine learning algorithms and evaluates their performance using classification metrics.

## Objectives

- Understand customer churn patterns through exploratory data analysis.
- Clean and prepare the dataset for machine learning.
- Analyze relationships between customer characteristics and churn.
- Train and compare multiple classification models.
- Evaluate model performance using accuracy, precision, recall, and F1-score.

## Dataset

**Dataset:** IBM Telco Customer Churn

The dataset contains customer demographic information, subscribed services, account details, billing information, and a target variable indicating whether a customer churned.

The `Churn` column is the target variable:
- `Yes`: The customer churned.
- `No`: The customer did not churn.

The `customerID` column is excluded from model training because it is an identifier.

## Project Workflow

1. Data loading and inspection
2. Data cleaning and handling missing values
3. Exploratory Data Analysis (EDA)
4. Feature selection and preprocessing
5. Train-test split
6. Machine learning model training
7. Model evaluation and comparison

## Exploratory Data Analysis

The analysis explores:
- Overall customer churn distribution
- Numerical feature distributions
- Churn rates across customer categories
- Customer tenure and churn patterns
- Contract types and payment methods
- Internet services and additional features

## Machine Learning Models

The following models are implemented:

1. Logistic Regression
2. Support Vector Machine (SVM)
3. Random Forest Classifier
4. XGBoost Classifier

### Feature Preprocessing

- **OneHotEncoder:** Encodes categorical input features.
- **StandardScaler:** Scales numerical features for Logistic Regression and SVM.
- **No StandardScaler:** Numerical features remain on their original scales for Random Forest and XGBoost.
- **LabelEncoder:** Encodes the target variable `Churn`.

Pipelines are used to keep preprocessing and model training organized.

## Evaluation Metrics

Model performance is evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted churners who actually churned.
- **Recall:** Proportion of actual churners correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Summary of correct and incorrect classifications.

The final model should be selected based on the evaluation results and the project's priorities, rather than accuracy alone.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost


## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/shahbaz-khan-ds/telecom-customer-churn-prediction.git
```



### 2. Navigate to the project directory

```bash
cd telecom-customer-churn-prediction
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
```

### 4. Download the dataset

Obtain the IBM Telco Customer Churn dataset and place the CSV file in the project directory, or update the notebook's data-loading path to match your dataset location.

### 5. Run the notebook

```bash
jupyter notebook Talecom_Customer_Churn2.ipynb
```

Run the notebook cells in order.

## Results

The notebook compares Logistic Regression, SVM, Random Forest, and XGBoost.

The final model comparison should report accuracy, precision, recall, and F1-score for each model. Actual performance values will be added after the notebook has been executed and the results verified.

## Future Improvements

- Perform cross-validation.
- Tune model hyperparameters.
- Investigate class imbalance.
- Compare precision-recall trade-offs.
- Evaluate feature importance and model interpretability.

## Disclaimer

This project is intended for educational purposes. Model predictions indicate patterns in historical data and should not be treated as guarantees of future customer behavior.
