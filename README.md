# Titanic Survival Prediction

## Overview
This project develops a machine learning model to predict passenger survival aboard the RMS Titanic. The goal is to preprocess the data and apply various classification algorithms to achieve the highest possible prediction accuracy.

## Data
The model is trained on classical built-in seaborn dataset.
-> https://www.kaggle.com/datasets/zain280/titanic-data-set

## Process
* **Data Exploration (EDA):** Investigated features, identified missing values in 'age' and 'embarked' columns.
* **Data Preprocessing:** Filled missing age values with the median, filled missing embarked with the mode, and one-hot encoded categorical features like 'sex' and 'embarked'.
* **Feature Engineering:** Created 'FamilySize' and 'IsAlone' features from 'sibsp' and 'parch' to test a new hypothesis.
* **Modeling & Tuning:** Used a Voting Classifier that combined both "Gradient Boosting Classifier", and "Random Forest Classifier", then used GridSearchCV to find the optimal hyperparameters.

## Results
* The final tuned ensemble model achieved an accuracy of 86.04% on the unseen test set.
* Feature importance analysis revealed that gender, passenger class, and fare were the most significant predictors of survival.

## Technologies Used
* Pandas
* NumPy
* Scikit-learn
* Seaborn
* Matplotlib
