# PS4E4 | Abalone Regression Dataset

## Introduction

This notebook explores the abalone dataset, which contains information about the age of abalone. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task. Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem.

## Data Description

The dataset consists of various measurements of abalone, including features such as length, diameter, height, and weight. These measurements are used as predictors to estimate the age of abalone. Additionally, categorical features such as sex are included in the dataset. The target variable, 'Rings', represents the age of abalone and is predicted based on the other features.

| Feature         | Type       | Description                            | Unit         | Categorical |
|-----------------|------------|----------------------------------------|--------------|-------------|
| Sex             | Categorical| M, F, and I (infant)                   |              | Yes         |
| Length          | Continuous | Longest shell measurement              | mm           | No          |
| Diameter        | Continuous | Perpendicular to length                | mm           | No          |
| Height          | Continuous | With meat in shell                     | mm           | No          |
| Whole_weight    | Continuous | Whole abalone                          | grams        | No          |
| Shucked_weight  | Continuous | Weight of meat                         | grams        | No          |
| Viscera_weight  | Continuous | Gut weight (after bleeding)           | grams        | No          |
| Shell_weight    | Continuous | After being dried                      | grams        | No          |
| Rings           | Integer    | +1.5 gives the age in years           |              | No          |

Reference: [Abalone Dataset](https://archive.ics.uci.edu/dataset/1/abalone)

## Approach

- Data loading and exploration: Load the dataset and perform initial exploration to understand its structure and content.
- Exploratory data analysis (EDA): Visualize the relationships between variables and gain insights into the data.
- Data preprocessing: Handle missing values, perform feature engineering, and prepare the data for modeling.
- Model building: Train and evaluate machine learning models to predict the age of abalone.
- Model evaluation: Assess the performance of the models using appropriate evaluation metrics such as accuracy, RMSLE, etc.

## Changes this version:

- Added the original data to improve performance.
- Dealt with the skewness transformation problem.
- Removed MinMaxScaling.
- Hyperparameter tuned LGBM model which achieved the best RMSLE so far on the LB.
