# Titanic Survival Prediction

## Overview
trying to make a model that predicts the survival of the titanic based on real-life data of the real passengers, and their survival state. The project aims to increase the accuracy score of predictions.

## Data
The model is trained on classical built-in seaborn dataset. 

## Process
* **Data Exploration (EDA):** Investigated features, identified missing values in 'age' and 'embarked' columns.
* **Data Preprocessing:** Filled missing age values with the median, filled missing embarked with the mode, and one-hot encoded categorical features like 'sex' and 'embarked'.
* **Feature Engineering:** Created 'FamilySize' and 'IsAlone' features from 'sibsp' and 'parch' to test a new hypothesis.
* **Modeling & Tuning:** Used a Voting Classifier that combined both "Gradient Boosting Classifier", and "Random Forest Classifierand", then used GridSearchCV to find the optimal hyperparameters.

## Results
* Achieved a final accuracy of ~84% on the test set.
* Feature importance analysis revealed that gender, passenger class, and fare were the most significant predictors of survival.

## Technologies Used
* Pandas
* NumPy
* Scikit-learn
* Seaborn
* Matplotlib
