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
