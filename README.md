# Diagnosing-Bias-and-Variance-in-Machine-Learning-Models

This repository contains code for building and evaluating linear regression models using various techniques such as polynomial regression, regularization (specifically Ridge regression), and learning curve analysis.

## Overview

The code in this repository is organized into several sections:

1. **Data Preparation**: 
    - Imports necessary libraries and utility functions.
    - Prepares datasets from CSV files using a utility function `prepare_dataset`.

2. **Linear Regression Modeling**:
    - Fits a linear regression model (`LinearRegression` from `sklearn.linear_model`) on a dataset.
    - Plots the training and cross-validation error against the degree of the polynomial.
    - Repeats the process with different bias values (`baseline`) to observe the impact on model performance.

3. **Regularization (Ridge Regression)**:
    - Demonstrates the use of Ridge regression by training models with different regularization parameters (`reg_params`) and visualizing their performance.
    - This is done for both datasets with varying degrees of polynomials.

4. **Dataset Comparison**:
    - Compares the performance of linear regression models on datasets with different numbers of features.
    - Plots the training and cross-validation errors for each dataset to observe how adding features affects model complexity and performance.

5. **Learning Curve Analysis**:
    - Analyzes the learning curve of the linear regression model.
    - Plots the training and cross-validation errors against the size of the training dataset.
    - Helps in understanding whether the model would benefit from additional data or if it suffers from high bias or high variance.

## Output
### Plot of Degree-of-polynomial-vs-train-and-CV-MSEs
![Degree-of-polynomial-vs-train-and-CV-MSEs](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/27ba87ae-81b5-4a82-878d-9d94f24cce22)

### Plot of degree of polynomial vs train and CV MSEs. Bias is define lower
![plot-of-degreee-of-polynomial-vs -train-and-CV-MSEs-Bias-is-define-lower](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/90c94c78-6a69-432c-8c24-47c581de7c41)

### Plot Degree of polynomial vs train and CV MSEs Dataset has two features
![Plot-Degree-of-polynomial-vs-train-and-CV-MSEs-Dataset-has-two-features](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/cb6a4b2c-557e-494e-a21f-893e471c2cbe)

### Plot lambda vs train and CV MSEs
![Plot-lambda-vs-train-and-CV-MSEs-](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/0c24e0df-ac0d-4281-8ca5-977c07f15688)

### Plot small values of lambda vs train and CV MSEs
![Plot-small-values-of-lambda-vs-train-and-CV-MSEs-](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/ed92010e-7802-4d51-b9ad-b33f073544a9)

### Plot Degree of polynomial vs train and CV MSEs for two datasets
![Plot-Degree-of-polynomial-vs-train-and-CV-MSEs-for-two-datasets](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/1080f6a0-c90b-42c4-b70a-bb6e0590b313)

### Plot of number of examples vs train and CV MSEs
![Plot-of-number-of-examples-vs-train-and-CV-MSEs](https://github.com/UMMY87/Diagnosing-Bias-and-Variance-in-Machine-Learning-Models/assets/117314436/b139e15f-340d-4fbb-8081-b5e91add52f4)


## Usage

To use this code:

1. Clone the repository.
2. Ensure you have the necessary dependencies installed (`numpy`, `pandas`, `scikit-learn`).
3. Run the Python script `linear_regression_analysis.py`.
4. View the generated plots and analyze the results.

## File Structure

- linear_regression_analysis.py     # Main Python script containing the analysis code
- utils.py                          # Utility functions for data preparation and plotting
- data/
    - c2w3_lab2_data1.csv           # Sample dataset 1
    - c2w3_lab2_data2.csv           # Sample dataset 2
    - c2w3_lab2_data3.csv           # Sample dataset 3
    - c2w3_lab2_data4.csv           # Sample dataset 4
- README.md                         # This README file


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
