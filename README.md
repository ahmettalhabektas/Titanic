# Titanic Data Analysis and Predictive Modeling

This Python code is an analysis and predictive modeling project on the Titanic dataset. The goal of this project is to explore the data, preprocess it, and build predictive models to determine the survival of passengers on the Titanic.

## Table of Contents

- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

The Titanic dataset is a classic dataset used for machine learning and data analysis. In this project, we perform data preprocessing, feature engineering, and build predictive models using various machine learning algorithms.

## Data Preprocessing

- Reading the train and test datasets.
- Merging the train and test datasets for a unified preprocessing.
- Handling missing values in the "Age" and "Fare" columns.
- Rounding "Age" values to improve data consistency.
- Encoding categorical variables like "Sex" and "Embarked."
- Creating a new feature "NumFamily" to represent the number of family members on board.
- Scaling the dataset using Min-Max scaling.
- Separating the train and test datasets.

## Feature Engineering

- Extracting titles from passenger names.
- Categorizing titles into meaningful groups based on age and gender.
- Imputing missing age values using the mean age of corresponding titles.
- Analyzing the distribution of cabin deck letters and handling missing values.
- Visualizing the dataset for better insights.

## Modeling

We explore several machine learning algorithms and choose the best-performing models:

- **Random Forest:** We fine-tune hyperparameters like criterion, max_depth, and n_estimators to achieve an accuracy of 0.79186.

- **Decision Tree:** We optimize hyperparameters like max_leaf_nodes, criterion, min_samples_leaf, and min_samples_split to reach an accuracy of 0.78229. We also visualize the decision tree.

- **Logistic Regression:** We experiment with different hyperparameters to achieve an accuracy of 0.77033.

- **Support Vector Machine (SVM):** We use the SVM algorithm with different hyperparameters and achieve an accuracy of 0.76794.

- **Voting Classifier:** We create a hard and soft voting classifier that combines the predictions of multiple models. The hard voting classifier achieves an accuracy of 0.78468, while the soft voting classifier achieves an accuracy of 0.77511.

## Results

We summarize the best results achieved with each algorithm:

| Algorithm            | Accuracy |
|----------------------|----------|
| Random Forest        | 0.79186  |
| Decision Tree        | 0.78229  |
| Hard Voting          | 0.78468  |
| Soft Voting          | 0.77511  |
| Logistic Regression  | 0.77033  |
| Support Vector Machine | 0.76794  |

## Conclusion

This code provides an in-depth analysis of the Titanic dataset, feature engineering, and modeling with various machine learning algorithms. The best-performing model is the Random Forest classifier with an accuracy of 0.79186. The decision tree and voting classifiers also show competitive results. Further improvements can be made by exploring additional feature engineering and hyperparameter tuning.

Feel free to adapt and extend this code for further analysis or use it as a reference for similar machine learning projects.
