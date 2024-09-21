# Heart Failure Prediction

## Problem Statement

With the vast availability of medical data and advancements in Data Science, many startups are tackling the challenge of predicting diseases before they occur. Cardiovascular diseases (CVDs) are the leading cause of death globally, accounting for 31% of all deaths worldwide. One common event caused by CVDs is heart failure. Individuals with cardiovascular disease or those at high cardiovascular risk (due to risk factors such as hypertension, diabetes, hyperlipidaemia, etc.) require early detection and management. Machine learning models can be pivotal in this process, providing early indications of potential heart failure, thereby aiding in proactive health interventions.

**Objective**:
- To predict whether a patient is prone to heart failure based on multiple attributes.
- This is a **binary classification** problem involving a mixture of numerical and categorical features.

## Table of Contents

1. [Data Overview](#data-overview)

2. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
    - [Categorical Features](#categorical-features)
    - [Numerical Features](#numerical-features)
    - [Target Variable Analysis](#target-variable-analysis)
    - [Relationships between Features](#relationships-between-features)

3. [Feature Engineering](#feature-engineering)

4. [Modeling](#modeling)
    - [Logistic Regression](#logistic-regression)
    - [Support Vector Classifier (SVC)](#support-vector-classifier-svc)
    - [Random Forest](#random-forest)
    - [XGBoost](#xgboost)

5. [Model Evaluation](#model-evaluation)

6. [Conclusion](#conclusion)

---

## Data Overview

We start by loading the necessary libraries and the dataset. Here's a summary of our data:
- **Columns and Data Info**: Displayed the column names and general information (i.e., null values, data types, etc.).
- **Missing Data Heatmap**: Visualized null values across features.
- **Statistical Summary**: Descriptive statistics of numerical columns using `.describe()` method.

---

## Exploratory Data Analysis (EDA)

### Categorical Features
We divide our data into categorical and numerical features, starting with an analysis of categorical features:
- **Distribution**: Displayed the frequency of each category within each feature.

- **Visualization**: Bar plots were used to illustrate categorical distributions.

### Numerical Features
Next, we explored the numerical features:

- **Descriptive Statistics**: Examined summary statistics for numerical columns.

- **Visualization**: Histograms were plotted to observe feature distributions.

### Target Variable Analysis

- **Target Counts**: Analyzed the class distribution of the target variable using a bar plot.

- **Percentage Distribution**: Visualized the proportion of each class using a pie chart.

### Relationships between Features

- **Categorical Features vs. Target**: Bar plots displaying the relationship between each categorical feature and the target variable.

- **Numerical Features vs. Target**: Count plots for each numerical feature against the target variable.

- **Categorical Features vs. Numerical Features (w.r.t Target)**: Visualizations showing relationships between categorical and numerical features, with the target variable considered.

- **Numerical Features vs. Numerical Features (w.r.t Target)**: Correlation matrices and scatter plots to explore relationships between numerical features.

### EDA Summary
- **Categorical Features (Order) :**
    - Sex : Male > Female
    - ChestPainType : ASY > NAP > ATA > TA
    - FastingBS : ( FBS < 120 mg/dl ) > ( FBS > 120 mg/dl)
    - RestingECG : Normal > ST > LVH
    - ExerciseAngina : Angina > No Angina
    - ST_Slope : Flat > Up > Down
 
- **Numerical Features (Range) :**
    - Age : 50+
    - RestingBP : 95 - 170 
    - Cholesterol : 160 - 340
    - MaxHR : 70 - 180
    - Oldpeak : 0 - 4

---

## Feature Engineering

- **Data Scaling**: Applied standard scaling techniques to normalize the numerical data.

- **Correlation Matrix**: Computed a correlation matrix to identify multicollinearity between features.

- **Chi-Square and ANOVA Tests**: Performed statistical tests (Chi-square for categorical features, ANOVA for numerical features) for feature selection.

---

## Modeling

We trained the following machine learning models:

### Logistic Regression

- **Accuracy**: Computed accuracy of the logistic regression model.

- **Cross-Validation Score**: Evaluated model performance using cross-validation.

- **ROC-AUC Score**: Calculated the ROC-AUC score for model assessment.

### Support Vector Classifier (SVC)

- **Accuracy**: Computed accuracy of the SVC model.

- **Cross-Validation Score**: Evaluated model performance using cross-validation.

- **ROC-AUC Score**: Calculated the ROC-AUC score for model assessment.

### Random Forest

- **Accuracy**: Computed accuracy of the Random Forest model.

- **Cross-Validation Score**: Evaluated model performance using cross-validation.

- **ROC-AUC Score**: Calculated the ROC-AUC score for model assessment.

### XGBoost

- **Accuracy**: Computed accuracy of the XGBoost model.

- **Cross-Validation Score**: Evaluated model performance using cross-validation.

- **ROC-AUC Score**: Calculated the ROC-AUC score for model assessment.

---

## Model Evaluation

For each model, we evaluated the performance based on:

- **Accuracy**

- **Cross-Validation Score**

- **ROC-AUC Score**

- **Confusion Matrix**: Plotted confusion matrices for each model.

Finally, we presented a **comparison table** of the models showing their key performance metrics.

---

## Conclusion

After evaluating multiple models, we found that the [best-performing model] based on [accuracy, cross-validation score, ROC-AUC] is [SVC]. The results suggest that this model is effective in predicting whether a patient is at risk of heart failure. Future improvements could include hyperparameter tuning, advanced feature engineering, or the inclusion of additional data to further enhance model performance.
