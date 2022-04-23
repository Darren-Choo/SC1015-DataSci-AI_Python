# SC1015 Mini Project

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on the World Happiness Report. 

Our group was interested in Singapores happiness score of 6.4, which was the highest amongst our immediate regional neighbours.

We wanted to abstract and utilise the important factors that affect the happiness score of a country, and use them to predict future data by training a model.


  
## Contributors

School of Computer Science and Engineering \
Nanyang Technological University \
Lab: DFS 2 \
Group : 3

Members: 
1. Darren Choo ([@Darren-choo](https://github.com/Darren-choo))
2. Cheong Jin Hui ([@jinhui18](https://github.com/jinhui18))
3. Darren Wong ([@darrenwwx](https://github.com/darrenwwx))

## Table of Contents:
1. [Problem Formulation](#Problem-Formulation)
2. [Data Preparation and Cleaning](#Data-Preparation-and-Cleaning)
3. [Exploratory Data Analysis](#Exploratory-Data-Analysis)
4. [Machine Learning](#Machine-Learning)
5. [Data Driven Insights and recommendations](#Data-Driven-Insights-and-recommendations)
6. [Key Learning Points](#Key-Learning-Points)
7. [References](#References)

## Problem Formulation
- To find out what variables are the most important in predicting life ladder.
- To build a model that best predicts the life ladder of different countries considering various regression models.

## Models Used

1. Multivariate Linear Regression 
2. Random Forest Regression
3. eXtreme Gradient Boosting Regression

## Data Preparation and Cleaning
In this section, we prepared and cleaned the dataset to help us retrieve variables that are useful for our project.

Carried out the following tasks:

1.	**Identifying** Irrelevant and relevant variables in our dataset. 
2.	**Visualised** missing data using the missingno Library.
3.	**Dropping** variables with more than 60% of missing data. 10 variables were dropped.
4.	**Filled** up the rest of the variables with missing data the **median** value.


## Exploratory Data Analysis
- Analysing and Comparing correlations before and after outlier removal.
- Comparing explained variance between each variable using univariate linear regression.
- Comparing explained variance with and without K-fold cross-validation

## Machine Learning

>|**Regression models**|
>|---|
>|Multivariate Linear Regression|
>|Random Forest Regressor|
>|eXtreme Gradient Boosting Regression|

## Data Driven Insights and recommendations
- Random forest regression is the best model to predict life ladder across all the 3 models we used.

## Key Learning Points
- Learnt to apply K-fold cross-validation in our project.
- Handling datasets with missing and irrelavant data.

## References
- https://worldhappiness.report/
