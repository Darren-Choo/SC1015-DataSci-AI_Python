# SC1015 Mini Project

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on the World Happiness Report. 

Our group was interested in Singapores happiness score of 6.4, which was the highest amongst our immediate regional neighbours.

We wanted to abstract and utilise the important factors that affect the happiness score of a country, and use them to predict future data by training a model.


  
## Contributors

School of Computer Science and Engineering \
Nanyang Technological University \
Lab: DFS 2 \
Group: 3

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

- Multivariate Linear Regression 
- Random Forest Regression
- eXtreme Gradient Boosting Regression

## Data Preparation and Cleaning
In this section, we prepared and cleaned the dataset to help us retrieve variables that are useful for our project.

Carried out the following tasks:

- **Identifying** Irrelevant and relevant variables in our dataset. 
- **Visualised** missing data using the missingno Library.
- **Dropping** variables with more than 60% of missing data. 10 variables were dropped.
- **Filled** up the rest of the variables with missing data the **median** value.


## Exploratory Data Analysis
In this section, we went on to analysed the relationship of the remaining variables with life ladder.

Carried out the following tasks:
- Analysed the correlation between the variables and Life Ladder.
  -Identified 3 variables with an extremely weak correlation with life ladder.
- Compared explained variance between each variable using univariate linear regression.
  - The same 3 variables had the lowest explained variance values, thus we decided to drop them. 
- Analysed and Compared correlations before and after outlier removal.
  - Evaluated that removal of outliers worsened the relationship between our variables and life ladder.
- Compared explained variance with and without K-fold cross-validation.

## Machine Learning

>|**Regression models**|**Hold-out cross validation**|**K-fold cross validation**|
>|---|---|---|
>|Multivariate Linear Regression| Explained Variance Score of **0.721** |Explained Variance Score of **0.753** |
>|Random Forest Regressor|Explained Variance Score of **0.863** |Explained Variance Score of **0.876** |
>|eXtreme Gradient Boosting Regression|Explained Variance Score of **0.791** |Explained Variance Score of **0.845** |

> #### Comparison of explained variance between the three models
> ![alt text](https://github.com/Darren-Choo/SC1015-DataSci-AI_Python/blob/main/Images/Comparison_of_models.png)
#### <br>

## Data Driven Insights and recommendations
- Random forest regression is the best model to predict life ladder across all the 3 models we used.
- Looking at the correlation and explained variance values of the variables in our dataset, we found the 3 most important variables in predicting life ladder.
  - Log GDP Per Capita
  - Social Support
  - Health Life Expectancy at birth
- Singapore should focus on improving these 3 components to achieve the highest increase in life ladder.

## Key Learning Points
- Learnt to apply K-fold cross-validation in our project.
- Handling datasets with missing and irrelevant data.

## References
- https://worldhappiness.report/
