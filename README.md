# E-commerce-and-banking-fraud-detection

## Project Overview

This project addresses the challenge of identifying fraudulent activities in two distinct domains: Credit Card Transactions and E-commerce Purchases. It aims to mitigate the annual loss of billions of dollars caused by financial fraud.

The primary goal is to build an automated pipeline capable of distinguishing between legitimate and fraudulent transactions. This is a Supervised Learning (Classification) problem characterized by extreme class imbalance, requiring specialized techniques to ensure accurate detection.


🏗️ Project Structure

```text

├── data/
│   ├── raw/              # Original datasets (Fraud_Data.csv, creditcard.csv, etc.)
│   └── processed/        # Cleaned and feature-engineered data
├── notebooks/
│   ├── eda-fraud-data.ipynb          # EDA for e-commerce fraud data
│   ├── eda-creditcard.ipynb          # EDA for credit card fraud data
│   ├── feature-engineering.ipynb    # Feature engineering and preprocessing
│   ├── modeling.ipynb                # Model training and evaluation
│ 
├── models/               # Saved trained models (.pkl files)
├── outputs/
│   └── eda/              # Visualizations organized by notebook
│       ├── creditcard/
│       ├── fraud-data/
│       ├── feature-engineering/
│       ├── modeling/
│       └── shap/
├── src/                  # Source code modules
├── scripts/              # Utility scripts
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

## 🚀 Setup Instructions

### Prerequisites

Python 3.8+

pip (Python package manager)


### Installation Steps

Clone the repository

```bash
git clone https://github.com/NaomiMeseret/E-commerce-and-banking-fraud-detection.git
cd E-commerce-and-banking-fraud-detection
```
Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment

macOS/Linux: ```bash source venv/bin/activate```

Windows: ```bash venv\Scripts\activate```

Install dependencies

```bash
pip install -r requirements.txt
```

# 🔍 Key Features

## 📊 Data Analysis & Engineering

Exploratory Data Analysis (EDA): In-depth univariate and bivariate analysis highlighting class imbalances.

Feature Engineering: * Time-based feature extraction.

Preprocessing: normalization, categorical encoding, and handling of missing values.

## 🤖 Model Building & Evaluation

Algorithms: Baseline Logistic Regression (with class balancing), Random Forest, and XGBoost.

Optimization: Hyperparameter tuning and Stratified K-Fold (k=5) cross-validation.

Metrics: Focused on AUC-PR and F1-Score to account for highly imbalanced fraud classes, alongside ROC-AUC and Confusion Matrices.


# Contributing

contributions are welcome! If you discover a bug or have a feature request, feel free to open an issue or submit a pull request.
