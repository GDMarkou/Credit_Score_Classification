# Credit Score Classification

This project was developed for the "Foundations of Machine Learning" course, part of the ESSEC & CentraleSupélec MSc in Data Science and Business Analytics program.

## Purpose 
The objective of this project is to classify bank customers into Credit Score categories (Bad, Standard, Good) based on a variety of features. Our goals are twofold: achieving the highest accuracy possible and exploring and evaluating multiple machine learning models. To meet these objectives, we followed this specific pipeline:

- Understanding our independent variables and the target variable.
- Preparing and processing our dataset.
- Conducting Feature Engineering and Feature Selection.
- Implementing Machine Learning Models, tuning Hyperparameters, and conducting Evaluation.

## Data

For the competition, we were provided with two datasets:
- **Training Set**: Contains the credit scores of customers.
- **Test Set**: Does not contain the credit scores of customers.

Throughout the competition, we did not have access to the labels of the test set. The performance of our model could only be evaluated by submitting our predictions to the Kaggle competition.

## Models and Methodology

We employed Stratified cross-validation and randomized grid search for hyperparameter tuning in all our models:
- Stratified CV is used as we are handling a classification problem. Without it, random data splitting could result in uneven distribution of labels. Stratified CV mitigates this risk.
- Randomized GridSearch is chosen to reduce training time, while identifying which parameters significantly impact model performance.

The models used in this project include:
- **Logistic Regression**
- **Random Forests**
- **XGBoost**
- **LightGBM**, best perfoming model.
- **Neural Networks (MLP)**

## Results

With strategic feature engineering and efficient hyperparameter tuning, we attained an accuracy of <b>86.44%</b>, using lightGBM, placing us 1st in the Kaggle Competition. Both the results and our methodology are available in this repository and are fully reproducible.