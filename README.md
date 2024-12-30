![image](https://github.com/user-attachments/assets/c2b20aa2-73e8-4e99-89d4-929f4767b95c)              ![image](https://github.com/user-attachments/assets/e5e4cf19-fd34-44f3-98ad-8f369703a787)



# Credit Risk Prediction Model
**Project-Based Internship Rakamin Academy X ID/X Partners**

This repository contains the implementation and documentation of a credit risk prediction model. The project is part of the final task of the Project-Based Internship in collaboration with Rakamin Academy and ID/X Partners.

The objective is to develop a machine learning model that can accurately predict credit risk based on loan application data. The project involves a complete end-to-end pipeline, including Data Understanding, Exploratory Data Analysis (EDA), Data Preparation, Data Modelling, Evaluation, and Model Improvement.

---

## Table of Contents
1. [Overview](#overview)
2. [Workflow](#workflow)
3. [Results](#results)
4. [File Structure](#file-structure)
5. [Prerequisites](#prerequisites)
6. [How to Use](#how-to-use)
7. [Repository Name Suggestion](#repository-name-suggestion)

---

## Overview

### Challenge  
The goal of this project is to help a multifinance company improve its decision-making process in assessing credit risk. By leveraging machine learning, the model will predict whether a borrower is likely to default based on historical data. Logistic Regression and Random Forest Classifier were used as the primary algorithms for this task.

### Dataset  
The dataset includes loan-related features such as the loan amount, interest rate, employment length, and more. Data preprocessing, including handling missing values and balancing the data, was a critical step in this project.

---

## Workflow

### 1. Data Understanding
- Analyzed dataset structure with 75 columns and 466,285 rows.
- Investigated column types, missing values, and overall statistics.

### 2. Exploratory Data Analysis (EDA)
- Visualized the distribution of loan statuses.
- Examined correlations between numerical features.
- Highlighted important patterns and trends in the data.

### 3. Data Preparation
- Imputed missing values.
- Encoded categorical features using Label Encoding.
- Scaled numerical features using StandardScaler.
- Addressed class imbalance with SMOTE.

### 4. Data Splitting
- Split data into training and testing sets with an 80:20 ratio.
- Applied SMOTE on the training data to balance the class distribution.

### 5. Data Modelling
- Developed two models:
  1. Logistic Regression: Focused on interpretability.
  2. Random Forest: Focused on higher accuracy and feature importance.

### 6. Evaluation
- Used metrics such as Confusion Matrix, ROC-AUC, and Precision-Recall curves.
- Compared the models’ performance:
  - Logistic Regression AUC: 0.78
  - Random Forest AUC: 0.97

### 7. Model Improvement
- Improved Logistic Regression by applying regularization and balancing class weights.
- Optimized Random Forest with hyperparameter tuning to enhance accuracy.

### 8. Final Model Deployment
- Saved the optimized models for future use (`optimized_logistic_regression.pkl` and `optimized_random_forest.pkl`).

---

## Results

### Key Insights
- Logistic Regression achieved good recall for classifying defaults but had limitations in precision.
- Random Forest significantly outperformed Logistic Regression, achieving an overall accuracy of 98%.

### Visualizations
- ROC Curves and Precision-Recall Curves were plotted for both models.
- Confusion Matrix Heatmaps and Classification Reports highlighted the performance differences.

---

## File Structure

- **Credit-Risk-Prediction/**
  - **data/**
    - `loan_data_2007_2014.csv`
  - **notebooks/**
    - `Credit_Risk_Prediction.ipynb`
  - **visualizations/**
    - `roc_curve_logistic_regression.png`
    - `roc_curve_random_forest.png`
    - `confusion_matrix_logistic_regression.png`
    - `confusion_matrix_random_forest.png`
  - `README.md`
  - `requirements.txt`





---

## Prerequisites

1. **Tools**  
   - Python 3.x  
   - Jupyter Notebook or Google Colab  

2. **Libraries**  
   - pandas, numpy, matplotlib, seaborn  
   - scikit-learn, imbalanced-learn  

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/username/Credit-Risk-Prediction.git
2. Install the required dependencies:
   
pip install -r requirements.txt

4. Run the Jupyter Notebook:

jupyter notebook notebooks/Credit_Risk_Prediction.ipynb

6. Explore the results and visualizations.
7. Access the models from the models/ directory for deployment.

**Link to Google Colab:** [Google Colab Notebook](https://colab.research.google.com/drive/11hZJTbWp3GuflhMoFV7Y7o4OKBXdzKeB?usp=sharing)
