# CreditWise Loan System

A Machine Learning-powered intelligent loan approval system for financial institutions.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Project Objectives](#project-objectives)
- [Dataset](#dataset)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)

---

## Overview

SecureTrust Bank is a mid-sized financial institution that offers personal and home loans to customers across urban and rural regions of India. With hundreds of loan applications daily through online and branch channels, the bank requires an intelligent, automated solution to streamline the loan approval process.

---

## Problem Statement

### Current Challenges

SecureTrust Bank currently relies on a **manual verification process** where loan officers evaluate applications by checking:

- Income proofs
- Employment details
- Credit history
- Supporting documents

### Issues with Manual Process

This time-consuming and manual approach leads to significant issues:

| Challenge                        | Impact                                             |
| -------------------------------- | -------------------------------------------------- |
| **Good customers rejected**      | Loss of business and market opportunity            |
| **High-risk customers approved** | Financial losses and increased default rates       |
| **Biased decisions**             | Inconsistent outcomes based on individual judgment |
| **Time-consuming**               | Slow turnaround time for customers                 |

---

## Solution

To address these challenges, SecureTrust Bank is implementing an **intelligent loan approval system** powered by Machine Learning that can:

✅ **Automatically analyze** applicant details  
✅ **Predict** loan approval or rejection with high accuracy  
✅ **Provide unbiased** decisions based on data patterns  
✅ **Ensure consistency** across all applications  
✅ **Enable faster** processing before final human verification

---

## Project Objectives

As a Machine Learning Engineer, the goal is to:

1. Design and develop an intelligent loan approval system
2. Learn hidden patterns from historical loan application data
3. Build a predictive model with high accuracy and reliability
4. Provide accurate, fast, and unbiased loan approval decisions
5. Support human verification with data-driven recommendations

---

## Dataset

The project uses historical loan application data to train the ML model. The dataset contains 20 features with applicant information and a target variable indicating loan approval status.

### Column Description

| Column | Description |
|--------|-------------|
| **Applicant_ID** | Unique applicant ID |
| **Applicant_Income** | Monthly income of applicant |
| **Coapplicant_Income** | Monthly income of co-applicant |
| **Employment_Status** | Salaried / Self-Employed / Business |
| **Age** | Applicant age |
| **Marital_Status** | Married / Single |
| **Dependents** | Number of dependents |
| **Credit_Score** | Credit bureau score |
| **Existing_Loans** | Number of already running loans |
| **DTI_Ratio** | Debt-to-Income ratio |
| **Savings** | Savings balance |
| **Collateral_Value** | Value of collateral provided |
| **Loan_Amount** | Loan amount requested |
| **Loan_Term** | Loan duration (months) |
| **Loan_Purpose** | Home / Education / Personal / Business |
| **Property_Area** | Urban / Semi-Urban / Rural |
| **Education_Level** | Graduate / Postgraduate / Undergraduate |
| **Gender** | Male / Female |
| **Employer_Category** | Govt / Private / Self |
| **Loan_Approved** (Target) | 1 = Approved, 0 = Rejected |

---

## Getting Started

### Files Included

- `code.ipynb` - Jupyter notebook with data analysis, model development, and evaluation
- `loan_approval_data.csv` - Historical loan application dataset
- `readme.md` - Project documentation

### Using the Notebook

1. Open `code.ipynb` in Jupyter Notebook or JupyterLab
2. Run cells sequentially to explore the data and train the model
3. Review model performance and predictions

---

## Project Structure

```
CreditWise Loan System/
├── code.ipynb                    # Main project notebook
├── loan_approval_data.csv        # Training dataset
└── readme.md                     # Project documentation
```

---

**Last Updated:** February 2026
