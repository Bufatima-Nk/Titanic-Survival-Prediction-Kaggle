# Titanic Survival Prediction Project

## Introduction

This repository contains the code and analysis for predicting passenger survival on the Titanic using data science techniques. The main objective of this project is to showcase my data preprocessing, exploration, model building, and evaluation skills.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Building](#model-building)
- [Model Evaluation](#model-evaluation)
- [Submission](#submission)
- [Files](#files)

## Data

The dataset used for this project is sourced from Kaggle and consists of two main files: `train.csv` and `test.csv`. The `train.csv` file contains information about passengers on the Titanic, including features like passenger class, sex, age, and fare. The goal is to predict whether a passenger survived or not, indicated by the 'Survived' column.

## Data Preprocessing

In the initial phase of the project, the data is read and cleaned using pandas. Columns that are unlikely to impact survival predictions, such as 'Ticket', 'Cabin', 'PassengerId', and 'Name', are dropped. Missing values in the 'Age' and 'Embarked' columns are imputed, and the data is prepared for analysis.

## Exploratory Data Analysis

Exploratory data analysis is carried out to gain insights into the dataset. Key visualizations include a count plot of survival, age distribution, survival percentage by gender, survival rate by passenger class, and port of embarkation distribution. The correlation heatmap and pair plot provide an understanding of feature relationships and their impact on survival.

## Model Building

A decision tree classifier model is chosen for predicting survival. The dataset is resampled using Random Over Sampling to balance the classes. A pipeline is built, including one-hot encoding, imputation, and the decision tree classifier. Hyperparameter tuning is performed using GridSearchCV to optimize the model's performance.

## Model Evaluation

The best model's accuracy is evaluated on a test set, resulting in an accuracy of approximately 0.79. A classification report provides precision, recall, and F1-score for both survival classes, and a confusion matrix visually represents the model's performance.

## Submission

The trained model is applied to the test dataset (`test.csv`) to generate predictions for passenger survival. The results are saved in a CSV file named `submission.csv` for submission to Kaggle's Titanic competition.

## Files

The repository contains the following files:

- `titanic-1.ipynb`: Jupyter Notebook containing the project code, including data preprocessing, exploratory data analysis, model building, and evaluation.
- `train.csv`: The training dataset containing passenger information.
- `test.csv`: The test dataset for generating predictions.
- `submission.csv`: CSV file containing predicted survival outcomes for the test dataset.
