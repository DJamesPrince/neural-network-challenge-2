# Neural Network Challenge 2: Employee Attrition and Department Prediction

## Overview

This project aims to create a neural network that predicts whether employees are likely to leave the company (attrition) and the department that best fits each employee. The predictions are made using a branched neural network.

## Table of Contents

- [Overview](#overview)
- [Files](#files)
- [Setup](#setup)
- [Instructions](#instructions)
- [Preprocessing](#preprocessing)
- [Model](#model)
- [Summary](#summary)

## Files

- `attrition.ipynb`: The main Jupyter notebook containing the code for data preprocessing, model creation, training, evaluation, and summary.
- [Dataset](https://static.bc-edx.com/ai/ail-v-1-0/m19/lms/datasets/attrition.csv): The dataset used for training and testing the model.

## Setup

1. Clone the repository to your local machine.
2. Upload `attrition.ipynb` to Google Colab or any other Jupyter Notebook environment.
3. Ensure you have the necessary libraries installed:
   - pandas
   - scikit-learn
   - tensorflow

## Instructions

Follow these steps in the notebook to complete the project:

### Part 1: Preprocessing

1. Import the data and view the first five rows.
2. Determine the number of unique values in each column.
3. Create `y_df` with the `Attrition` and `Department` columns.
4. Create a list of at least 10 column names to use as X data.
5. Create `X_df` using your selected columns.
6. Show the data types for `X_df`.
7. Split the data into training and testing sets.
8. Convert your X data to numeric data types as necessary.
9. Create a `StandardScaler`, fit the scaler to the training data, and transform both the training and testing data.
10. Create a `OneHotEncoder` for the department column, fit the encoder to the training data, and transform both the training and testing data.
11. Create a `OneHotEncoder` for the attrition column, fit the encoder to the training data, and transform both the training and testing data.

### Part 2: Create, Compile, and Train the Model

1. Find the number of columns in the X training data.
2. Create the input layer. Do NOT use a sequential model, as there will be two branched output layers.
3. Create at least two shared layers.
4. Create a branch to predict the department target column. Use one hidden layer and one output layer.
5. Create a branch to predict the attrition target column. Use one hidden layer and one output layer.
6. Create the model.
7. Compile the model.
8. Summarize the model.
9. Train the model using the preprocessed data.
10. Evaluate the model with the testing data.
11. Print the accuracy for both department and attrition.

### Part 3: Summary

Answer the following questions in the notebook:

1. Is accuracy the best metric to use on this data? Why or why not?
2. What activation functions did you choose for your output layers, and why?
3. Can you name a few ways that this model could be improved?

## Preprocessing

The preprocessing steps include importing the data, creating the target and feature datasets, encoding categorical data, scaling numerical data, and splitting the data into training and testing sets.

## Model

The model consists of an input layer, shared hidden layers, and two output branches: one for predicting the department and one for predicting attrition. The model is compiled, trained, and evaluated on the preprocessed data.

## Summary

The summary section provides answers to key questions about the model's performance and potential improvements.


Leveraged ChatGPT for Readme and for the Project where I needed help.

