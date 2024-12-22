# Loan Eligibility Prediction Model

This repository contains the code and documentation for a Machine Learning model designed to predict loan eligibility. The solution includes data preprocessing, exploratory data analysis (EDA), model training using Vertex AI, and performance evaluation.

---

## Table of Contents
- [Project Structure](#project-structure)
- [Overview](#overview)
- [Data Preprocessing and EDA](#data-preprocessing-and-eda)
- [Model Training](#model-training)
- [Performance Metrics](#performance-metrics)
- [Feature Importance](#feature-importance)

---

## Project Structure
```bash
├── code
│   └── loan-eligibility-data-pre-processing-and-eda.ipynb
├── data
│   ├── 
├── README.md
└── artifacts
    └── FinalSolutionSlideDeckpptx.pptx
    └── Solution Approach Document.pdf
```
---

## Overview
The project aims to predict loan eligibility by analyzing applicant data using a Machine Learning model. The model's primary goal is to minimize false positives (approving loans for ineligible applicants) to reduce the risk for lenders.

---

## Data Preprocessing and EDA
The dataset was thoroughly explored through Exploratory Data Analysis (EDA) and prepared for processing in Jupyter Notebooks. Key steps included:
- Identifying and handling missing values
- Transforming categorical variables
- Scaling numerical features

All EDA and preprocessing steps are documented in the solution approach document, and the corresponding code is available in the `Final Solution` folder.

---

## Model Training
The prepared dataset was used to train the model using Google's Vertex AI platform. Performance metrics, including PR and ROC Curves, were evaluated at a confidence threshold of 0.5.

---

## Performance Metrics
The model's performance was assessed using a confusion matrix:
- **True Negative Rate (Denying Loans Correctly):** 97%
- **False Negative Rate (Denying Eligible Loans):** 57%
- **False Positive Rate (Approving Ineligible Loans):** 3%
- **True Positive Rate (Approving Eligible Loans):** 43%

While the false negatives were relatively high, the low false positive rate ensures minimal risk to the bank by reducing the likelihood of granting loans to ineligible applicants.

---

## Feature Importance
The most significant features influencing the model's predictions were:
1. **Interest Rate**
2. **Grade** (based on the applicant’s credit history)
3. **Last Payment Week** (`last_week_pay`)

These features were determined to be critical in predicting loan outcomes.

---

## Usage
1. Clone this repository.
2. Navigate to the `Final Solution` folder.
3. Execute the Jupyter Notebooks to explore the EDA and model training process.

--- 

For more details, refer to the solution approach document and the `Final Solution` folder.
