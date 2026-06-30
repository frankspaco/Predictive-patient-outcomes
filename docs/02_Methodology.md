# Methodology

## 1. Data Preparation

The project used patient encounter data containing healthcare, admission, medication and readmission-related variables.

The dataset required preprocessing before machine learning could be applied. This included replacing invalid placeholder values with missing values, assessing missing data, removing unreliable columns and imputing missing categorical values using the mode.

## 2. Feature Engineering

Additional features were created to improve the modelling process, including:

- Binning `time_in_hospital` into categories
- Creating an interaction feature between medication count and hospital stay duration
- Encoding categorical variables
- Scaling numerical features using `StandardScaler`

## 3. Model Development

Two supervised machine learning models were developed:

- Logistic Regression
- Random Forest Classifier

The models were trained using an 80/20 train-test split.

## 4. Model Evaluation

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

## 5. Model Improvement

The Random Forest model was further improved using:

- Feature importance analysis
- Top feature selection
- GridSearchCV hyperparameter tuning

## 6. Explainability

SHAP was explored to interpret model predictions and understand how selected features contributed to individual predictions.
