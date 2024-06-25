# QUIZ-6-7
For this exercise i use database frin keggle - World_Billionaire_2024.csv
LINK - https://www.kaggle.com/datasets/divanshu22/richest-people-in-the-world-2024?resource=download

First exercise:
Data Loading and Cleaning:
Load the CSV file.
Skip the first row to get the correct headers.
Clean the NET WORTH column by removing dollar signs and the letter 'B' to convert it into numerical format.
Defining Features and Target:
Use RANK as the feature (independent variable).
Use NET WORTH as the target (dependent variable).
Train-Test Split:
Split the dataset into training and testing sets.
Model Training and Evaluation:
Train a LinearRegression model.
Make predictions on the test set.
Calculate the Mean Squared Error (MSE) and R-squared value to evaluate the model.
Visualization:
Plot the actual vs. predicted values for the test set.
Testing on New Data:
Make predictions on new data with ranks 50, 100, and 150.



Second:
I made everything same but on new date I made next steps:
Create new data with specified ranks and countries.
 Ensure the new data has all necessary columns and in the same order as the training data.
Make predictions on the new data.



THIRD:

Encoding Categorical Variables:
One-hot encode the COUNTRY column.
Defining Features and Target:
For single variable regression, use RANK as the feature.
For multiple variable regression, use RANK and the one-hot encoded country columns as features.
Use NET WORTH as the target variable.
Function for Decision Tree Regression:
Split the dataset into training and testing sets.
Train a DecisionTreeRegressor model.
Make predictions on the test set.
Calculate the Mean Squared Error (MSE) and R-squared value to evaluate the model.
Test the model on new data.
 Testing on New Data:
Create new data with specified ranks and countries.
Ensure the new data has all necessary columns and in the same order as the training data.
Make predictions on the new data.


FIFTH:
Data Preparation: Columns are cleaned to remove any leading or trailing whitespaces using data.columns.str.strip().
 Feature Selection: For illustration purposes, X is defined as 'RANK' and 'NET WORTH', which are features used to predict the country (COUNTRY).
Model Training: A Decision Tree Classifier is initialized and trained using X_train and y_train.
Model Evaluation: Predictions are made on X_test, and metrics such as accuracy are calculated using accuracy_score. The classification_report provides detailed metrics including precision, recall, and F1-score.
Prediction on New Data: Demonstrates how to prepare and predict on new data (new_data). The model predicts the country (COUNTRY) based on the 'RANK' and 'NET WORTH' provided in new_data.

