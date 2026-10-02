# Stroke Risk Prediction

A predictive analytics project using machine learning to explore stroke-risk prediction from structured healthcare data.

This project was completed for **NIT3151 – Predictive Analytics** at Victoria University.

## Project Overview

The objective of this project was to develop and evaluate machine learning models for predicting whether a patient may be at risk of stroke based on healthcare and demographic attributes.

The workflow included:

- Data exploration
- Data cleaning and preprocessing
- Handling missing values
- Preparing categorical and numerical features
- Addressing class imbalance
- Model training and tuning
- Model evaluation
- Confusion-matrix analysis
- Comparing models using metrics appropriate for an imbalanced healthcare dataset

## Dataset

The dataset contains healthcare and demographic attributes including:

- Gender
- Age
- Hypertension
- Heart disease
- Marital status
- Work type
- Residence type
- Average glucose level
- BMI
- Smoking status
- Stroke outcome

The target variable is:

`stroke`

where the model attempts to distinguish stroke and non-stroke cases.

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
- imbalanced-learn
- SMOTE

## Machine Learning Workflow

### 1. Data Preparation

The dataset was inspected and cleaned before modelling.

Tasks included:

- Checking missing values
- Preparing numerical and categorical variables
- Producing a cleaned dataset
- Preparing features for machine learning

### 2. Class Imbalance

Stroke cases represent a much smaller proportion of the dataset than non-stroke cases.

Because of this imbalance, the project used **SMOTE (Synthetic Minority Over-sampling Technique)** within the modelling workflow to improve learning from the minority class.

## Model Evaluation

The project evaluated model performance using multiple metrics rather than relying only on accuracy.

Metrics included:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC
- Confusion Matrix

Recall was particularly important because, in this type of prediction task, identifying more of the actual positive stroke cases is valuable for model comparison.

## Result

The final model comparison recommended **Logistic Regression** based on test-set recall.

The tuned Logistic Regression model achieved approximately:

- **Accuracy:** 0.74
- **Precision:** 0.14
- **Recall:** 0.82
- **F1 Score:** 0.24
- **ROC AUC:** 0.84

These results also demonstrate the difficulty of modelling a highly imbalanced healthcare dataset: strong recall can come with lower precision.

This project is an academic predictive-modelling exercise and is **not intended for clinical diagnosis or medical decision-making**.

## Repository Contents

### `Final_version.ipynb`

Main Jupyter Notebook containing:

- Data preprocessing
- Exploratory analysis
- Class-imbalance handling
- Model training
- Model tuning
- Model evaluation
- Confusion matrices
- Final model comparison

### `healthcare-dataset-stroke-data.csv`

Original dataset used for the project.

### `stroke_data_cleaned.csv`

Cleaned version of the dataset produced during preprocessing.

### `NIT3151 Assessment 2 Report - Final.docx`

Written project report describing the methodology, analysis and findings.

## My Contribution

This was a group project.

According to the project workflow, my main responsibility covered **Steps 5–8**, including later-stage predictive modelling, model evaluation and analysis.

## Skills Demonstrated

- Predictive analytics
- Machine learning
- Healthcare data analysis
- Data preprocessing
- Class-imbalance handling
- SMOTE
- Model evaluation
- Hyperparameter tuning
- Confusion-matrix interpretation
- Recall, precision, F1 and ROC AUC analysis
- Python and Jupyter Notebook

## Limitations

- The dataset is highly imbalanced.
- Predictive performance depends on the available features and dataset quality.
- The project was developed for academic purposes.
- The model should not be interpreted as a clinical diagnostic system.

## Future Improvements

Potential improvements include:

- Testing additional machine learning algorithms
- Comparing alternative imbalance-handling techniques
- Improving feature engineering
- Performing feature-importance analysis
- Testing additional cross-validation strategies
- Evaluating model calibration
- Exploring threshold optimisation for recall and precision

## Author

**Justin Dang**

Bachelor of Data Science  
Victoria University
