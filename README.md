# Predictive Patient Outcomes Using Machine Learning

## Project Features

✔ Healthcare data preprocessing

✔ Data quality assessment

✔ Missing value handling

✔ Feature engineering

✔ Machine Learning modelling

✔ Model comparison

✔ Performance evaluation

✔ Reproducible workflow


This project was completed as part of my MSc in Applied Artificial Intelligence and Data Analytics. It explores how machine learning can be used to predict patient outcomes using healthcare data.

## Portfolio Note

This project was originally completed as part of my MSc in Applied Artificial Intelligence and Data Analytics. The repository has since been reorganised and documented to present the work clearly as part of my professional data portfolio.

The project involved preparing and analysing patient-related data, building predictive models, and evaluating model performance using appropriate machine learning metrics.

## Project Aim

The aim of this project was to investigate whether machine learning models could support the prediction of patient outcomes by identifying patterns in historical healthcare data.

## Dataset

The original dataset used for this project is not included in this repository.

During the MSc dissertation, the dataset was processed and transformed to create a modified dataset for machine learning analysis. This involved data cleaning, preprocessing and feature engineering to prepare the data for Logistic Regression and Random Forest modelling.

The repository is therefore intended to showcase the machine learning workflow, Python implementation, model development and evaluation process rather than provide a fully reproducible dataset package.

## Data Preparation

The dataset contained patient encounter information, including admission details, medication indicators and readmission status.

Additional synthetic features were created for modelling purposes, including:

- **Age** – generated numeric age values between 20 and 90.
- **Gender** – generated categorical gender values.
- **Has_Diabetes** – generated a binary diabetes indicator using an assumed prevalence of 20%.

A fixed random seed was used to ensure the synthetic feature generation was reproducible.

The dataset was then prepared for machine learning through preprocessing and feature engineering.

## Data Cleaning Process

The healthcare dataset required preprocessing before machine learning could be performed.

The data preparation process included:

- Replacing invalid placeholder values ('?') with missing values (NaN)
- Assessing missing values across all variables
- Creating a processed dataset for modelling
- Generating additional synthetic patient features
- Exporting the cleaned dataset for downstream analysis

These preprocessing steps ensured the data was suitable for machine learning and demonstrated practical data preparation techniques commonly used in real-world analytical workflows.

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn

## Models Used

- Logistic Regression
- Random Forest Classifier

## Model Evaluation

The models were evaluated using standard classification metrics:

- Accuracy
- Weighted Precision
- Weighted Recall
- Weighted F1-score

Weighted averages were used to account for class distribution across the target variable.

The notebook also supports visual evaluation using confusion matrices and ROC curves.

## Model Performance

The initial predictive models were evaluated using standard classification metrics.

| Metric | Result |
|---------|---------:|
| Accuracy | 53.83% |
| Weighted Precision | 44.98% |
| Weighted Recall | 53.83% |
| Weighted F1 Score | 44.53% |

These results provided a baseline for comparing predictive models and highlighted opportunities for further optimisation through feature engineering, hyperparameter tuning and improved handling of class imbalance.

## Challenges Encountered

During model evaluation, the initial Logistic Regression model produced class imbalance warnings, resulting in an `UndefinedMetricWarning` for precision on some classes.

This highlighted the challenges associated with imbalanced healthcare datasets, where certain outcome classes were underrepresented.

The evaluation process reinforced the importance of:

- Understanding class imbalance
- Selecting appropriate evaluation metrics
- Interpreting model performance beyond overall accuracy
- Considering alternative modelling and balancing techniques for future improvements

## Skills Demonstrated

### Data Engineering

- Data extraction
- Data transformation
- Dataset creation
- Data export
- Missing value handling
- Data quality assessment

### Data Analysis

- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Cleaning
- Statistical Analysis

### Machine Learning

- Logistic Regression
- Random Forest
- Model Evaluation
- Classification Metrics
- ROC Analysis
- Confusion Matrix

### Programming

- Python
- Pandas
- NumPy
- Scikit-learn

## Project Workflow

1. Loaded patient encounter data containing hospital admission, medication and readmission variables.
2. Created additional synthetic patient-level features to support modelling.
3. Removed unreliable columns and handled missing values.
4. Encoded categorical variables using one-hot encoding and label encoding.
5. Scaled numerical features using standardisation.
6. Split the dataset into training and testing sets.
7. Trained Logistic Regression and Random Forest models.
8. Evaluated model performance using classification metrics, confusion matrices and ROC curves.
9. Compared model performance and interpreted the results.

## Feature Engineering and Preprocessing

After missing values were handled, the dataset was prepared for machine learning through feature encoding and scaling.

The preprocessing steps included:

- Dropping the `weight` column due to missing or unreliable values.
- Imputing missing values in selected categorical columns using the mode.
- Applying one-hot encoding to categorical variables with limited unique values.
- Applying label encoding to categorical variables with many unique values.
- Scaling numerical features using `StandardScaler`.
- Splitting the dataset into training and testing sets using an 80/20 split.

These steps ensured that the dataset was converted into a suitable numerical format for Logistic Regression and Random Forest modelling.

## Results

The project compared the predictive performance of Logistic Regression and Random Forest models for patient outcome prediction.

Performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC Curve
- Confusion Matrix

The notebook automatically generates evaluation metrics and visualisations, allowing the complete model assessment process to be reproduced.

## Key Learning

This project strengthened my understanding of the full machine learning workflow, from data preparation through to model evaluation. It also helped me appreciate the importance of data quality, feature selection and responsible use of predictive analytics in healthcare-related contexts.

## Repository Contents

- `logistic_regression_and_random_forest_model.ipynb` — main machine learning notebook
- `README.md` — project documentation

## Author

Frank Adiela  
MSc Applied Artificial Intelligence and Data Analytics  
Aspiring Data Engineer / AI Engineer
