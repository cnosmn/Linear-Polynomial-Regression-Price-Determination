# Linear and Polynomial Regression Analysis

[![Python](https://img.shields.io/badge/Python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24-green.svg)](https://scikit-learn.org/stable/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3-yellow.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11-red.svg)](https://seaborn.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## Overview

This repository demonstrates the implementation and comparison of Linear Regression and Polynomial Regression models for predicting sales based on advertising expenditures. Through practical examples, the project highlights the differences in accuracy between these two regression techniques and showcases model tuning and evaluation methods.

## Table of Contents

- [Linear and Polynomial Regression Analysis](#linear-and-polynomial-regression-analysis)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Dataset](#dataset)
  - [Models](#models)
  - [Features](#features)
  - [Results](#results)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Dependencies](#dependencies)

## Introduction

Regression analysis is a fundamental technique in predictive modeling that estimates relationships between variables. This project focuses on:

1. Simple Linear Regression: Modeling the relationship between a single predictor variable and the target
2. Multiple Polynomial Regression: Modeling relationships using multiple predictor variables
3. Comparing model performance through error metrics

## Dataset

The analysis uses the "Advertising.csv" dataset which contains information about advertising expenditures across different media channels and their impact on sales:

- **TV**: Advertising budget spent on TV commercials (in thousands of dollars)
- **Radio**: Advertising budget spent on radio commercials (in thousands of dollars)
- **Newspaper**: Advertising budget spent on newspaper ads (in thousands of dollars)
- **Sales**: Number of products sold (in thousands of units)

## Models

The repository implements and compares two regression models:

1. **Simple Linear Regression**: Using only TV advertising to predict sales
   - Mathematical form: Sales = 7.03 + 0.05 × TV

2. **Multiple Polynomial Regression**: Using all advertising channels (TV, radio, and newspaper) to predict sales
   - Mathematical form: Sales = 2.94 + 0.046 × TV + 0.189 × Radio - 0.001 × Newspaper

## Features

- Data loading and preprocessing
- Exploratory data analysis with visualization
- Simple linear regression model implementation
- Multiple polynomial regression model implementation
- Model performance comparison using error metrics
- Sales prediction for new advertising budget scenarios
- Detailed visualization of regression models

## Results

The analysis shows that the polynomial regression model outperforms the linear regression model:

- **Linear Regression R²**: 0.612 (explains 61.2% of the variance in sales)
- **Polynomial Regression R²**: 0.897 (explains 89.7% of the variance in sales)
- **Linear Regression MSE**: 9.29
- **Polynomial Regression MSE**: 5.02

The comparison demonstrates that considering multiple advertising channels in the model (TV, radio, and newspaper) provides significantly better predictive power than using TV advertising alone.

## Installation

1. Clone this repository
```bash
git clone https://github.com/cnosmn Linear-Polynomial-Regression-Price-Determination.git
cd Linear-Polynomial-Regression-Price-Determination
```

2. Install required packages
```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

## Usage

1. Load the Jupyter Notebook or Python script in your preferred environment
2. Run all cells sequentially to see the complete analysis
3. Modify the input values in the prediction sections to test different advertising budget scenarios

## Dependencies

- Python 3.x
- pandas: For data manipulation and analysis
- scikit-learn: For implementing regression models
- seaborn & matplotlib: For data visualization
- numpy: For numerical operations

---

Feel free to contribute to this repository by adding more regression techniques or improving the existing models. If you have any questions or suggestions, please open an issue or submit a pull request.