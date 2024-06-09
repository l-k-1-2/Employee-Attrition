# Employee Attrition Prediction

Employee attrition prediction is a valuable tool for management. It helps in predicting the chances of an employee leaving the company and preparing accordingly to ensure a smooth transition or retention of employees. Key factors involved in employee attrition, such as salary, age, work experience, can be predicted using data available from the Human Resources Management (HRM) team.

In this project, we work with a dataset of employees from IBM and aim to predict if an employee will leave the company.

## Objective

The objective of this project is to deeply analyze the available data, clean it, and build a model to predict employee attrition.

## The Project

### Database Description and Preprocessing
The dataset used for this project consists of 35 factors recorded for 1470 employees from IBM. The data is abstract, and some preprocessing was required. We encoded categorical data like gender, department, marital status using Label Encoder. We dropped columns like employee count, standard hours, and over 18, as they had the same values across all rows.

### Model Selection
Based on the given case, we selected four models: Logistic Regression, Decision Tree Classifier, K-Nearest Neighbor, and Random Forest Classifier. We performed cross-validation, random undersampling, and random oversampling to determine which model performs best for the given dataset. Using metrics like mean score, z-score, and recall score, we determined that Logistic Regression is the best performing model.

Understandably, Logistic Regression stands out as the best-performing model, as it fulfills the assumptions made by the data, such as a binary target variable, independent observations, sample size, number of outliers, etc.

### Model Preparation and Results
With the model decided, we conducted Exploratory Data Analysis (EDA) to identify the factors that have the most impact on employee attrition. We used a correlation matrix to determine the factors with high or low impact on attrition. We then individually visualized these impactful factors to gain a better understanding of their relationship with attrition. We selected the most impactful factors for modeling.

The dataset was randomly split into 70% for training and 30% for testing. We trained and tested our model and calculated its performance using a confusion matrix. We achieved a training accuracy of 88.9% and a testing accuracy of 86.8%.

