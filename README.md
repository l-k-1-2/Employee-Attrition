# EDA and Attrition Prediction of Employees

Prediction of employee attrition is a very helpful tool for management. It can help in predicting the chances of an employee leaving the company and prepare accordingly to ensure smooth transitioning / retention of employees. A lot of factors are involved in employee attrition, like salary, age, work experience, etc. Data related to a lot of these key parameters is avaialble with the Human Resources Management (HRM) team and could be helpful in predicting employee attrition.

In this project, we work with one such dataset and predict if an employee will leave the company or not. 

## Objective

The objective of this project is to take a deep dive into the available data, analyze and clean it, and then build a model to predict employee attrition.

## The Project

### Database description and pre-processing
The database taken for this project is a dataset of employees from IBM where as many as 35 factors are recorded for 1470 employees. The data is rather abstract and some pre-processing was required on the dataset. We encoded the categorical data like gender, department, marital status, etc using Label Encoder. We dropped columns like employee count, standard hours, and over 18 as they had the same values across all rows.

### Model Selection
Based on the used case, we shortlisted 4 models - Logistic Regression, Decision Tree Classifier, K-Nearest Neighbor and Random Forest Classifier. We then prformed cross validation, random undersampling and random oversampling to predict which model is performing the best for the given data. Using metrics of mean score, z-score and recall score, we determined that Logistic Regression is the best performing model for the given dataset.

The standing out of logistic regression is understandable as a lot of assumptions taken in logistic regression are fulfilled by the data set like:
* Target variable is categorical and binomial
* The observations are largely independent of each other
* Sample size is considerable with limited outliers

All these factors support Logistic regression to turn out as the best performing model.

### Model Preparation and Results
With the model decided, we proceeded with EDA to determine the factors which impact attrition the most. Using correlation matrix we determined the factors which have very high or very low impact on attrition. We then individually visualized the impactful factors to get a better understanding of the relation of these factors with attrition. We shortlisted the most impactful factors from the analysis and considered them for modeling.

The dataset was randomly split in 70:30 ratio for training and testing respectively. We trained and tested our model and calculated the performance with help of confusion matrix. We achieved a training accuracy of 88.9% and testing accuracy of 86.8%.
