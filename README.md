# Diabetes-Regression-Models-Evaluation

This repository contains a Python script that evaluates various regression models using the Diabetes dataset from the `scikit-learn` library. The script performs data preprocessing, trains multiple regression models, and evaluates their performance using common metrics.

## Table of Contents

- Overview
- Requirements
- Data
- Usage
- Script Details
  - Data Loading
  - Data Preprocessing
  - Model Training and Evaluation
  - Metrics
- License

## Overview

The script demonstrates how to:

1. Load and preprocess the Diabetes dataset.
2. Train different regression models on the dataset.
3. Evaluate and compare the performance of these models.

## Requirements

To run this script, you'll need Python 3.x and the following libraries:

- `numpy`
- `pandas`
- `scikit-learn`

## Script Details

### Data Loading

The script loads the Diabetes dataset from `scikit-learn` and creates a DataFrame for easier handling:

```python
from sklearn.datasets import load_diabetes
import pandas as pd

# Load the Diabetes dataset
diabetes = load_diabetes()

# Create a DataFrame
df = pd.DataFrame(diabetes.data, columns=diabetes.feature_names)

# Display the first few rows of the DataFrame
df.head().T
```

## Script Details
# Data Loading
The script loads the Diabetes dataset and creates a DataFrame for easier handling.

###Data Preprocessing
#Normalization: The feature data is normalized to ensure that all features have the same scale.

# Model Training and Evaluation
The script trains and evaluates the following regression models:

- Linear Regression
- Lasso Regression
- Ridge Regression
(Note: Logistic Regression is excluded as it is intended for classification tasks, not regression.)

# Metrics
The performance of each model is evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R-Squared (R²)
These metrics help in assessing the model's accuracy and predictive power.

# Results
After execution, the script prints the performance metrics for each model, providing a comparison of how well each model performs on the test set.
