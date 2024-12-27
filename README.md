# Loan Repayment Prediction Model using LSTM-CNN Technique

This repository contains a machine learning model developed to predict loan repayment behavior using a hybrid Long Short-Term Memory (LSTM) and Convolutional Neural Network (CNN) approach. The model is designed to predict whether a borrower will repay a loan or default based on various financial and behavioral factors. By leveraging both sequential and feature extraction techniques, the LSTM-CNN model provides a robust solution for assessing credit risk and enhancing decision-making in financial institutions.

The model analyzes historical loan data, borrower demographics, financial behavior, and loan details to make predictions. This approach aims to improve the accuracy of loan repayment predictions, helping financial organizations reduce the risk of defaults and optimize their lending strategies.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Requirements](#requirements)
- [Setup](#setup)
- [Training](#training)
- [Evaluation](#evaluation)
- [Usage](#usage)


## Project Overview

The Loan Repayment Prediction Model utilizes a combination of LSTM and CNN layers to address the complexities of predicting loan repayment behavior. LSTM is well-suited for modeling sequential data, such as historical payment patterns, while CNN helps in identifying relevant features and patterns that could indicate the likelihood of loan repayment or default.

This model can be used by banks, financial institutions, and lending platforms to improve their loan approval processes, reduce financial risks, and make more informed decisions based on predictive insights.

## Features

The model considers the following features for predicting loan repayment:

- **Demographic Information**: Age, income, marital status, etc.
- **Financial History**: Previous loan repayment status, credit score, etc.
- **Loan Characteristics**: Loan amount, interest rate, term, etc.
- **Behavioral Data**: Spending patterns, account activity, etc.

These features are carefully selected to represent both the financial behavior of the borrower and the characteristics of the loan itself.

## Model Architecture

The architecture is a hybrid of LSTM and CNN layers:

1. **LSTM Layer**: Captures sequential dependencies from the data, such as the borrower’s past payment history.
2. **CNN Layer**: Extracts key features from the data to identify patterns in loan repayment behavior.
3. **Fully Connected Layers**: Outputs the prediction of loan repayment (repay or default).

### Model Workflow:

- The sequential data is passed through the LSTM layer to learn temporal patterns in loan repayment.
- The CNN layer processes the output of the LSTM to extract important features.
- Finally, the dense layers make the final prediction of whether the borrower will repay the loan or default.

## Requirements

To run this project, you will need the following libraries:

- Python 3.x
- TensorFlow
- Keras
- Pandas
- Numpy
- Scikit-learn
- Matplotlib
- Seaborn

You can install these dependencies by running:

```bash
pip install -r requirements.txt
