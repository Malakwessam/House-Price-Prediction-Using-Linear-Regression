# House-Price-Prediction-Using-Linear-Regression
A regression project that predicts house prices using simple and multiple linear regression, comparing model performance and analyzing the impact of socioeconomic factors on housing values.



##  Overview

The goal of this project is to predict house prices using real-world features such as income level, number of rooms, pollution, and educational ratios.

The project compares:

- Simple Linear Regression (single feature)  
- Multiple Linear Regression (multiple features)  

to evaluate how additional variables improve prediction accuracy.



##  About the Dataset

The dataset contains **506 records and 14 features**, including:

- Crime rate (CRIME)  
- Residential zones (ZONE)  
- Industrial areas (INDUS)  
- Pollution level (POLLUTION)  
- Number of rooms (ROOM)  
- Age of houses (AGE)  
- Distance to employment (DIS_JOB)  
- Tax rates (TAX)  
- Student-teacher ratio  
- Lower income percentage (LSTAT)  
- Target: **Median house value (MED_HOUSE_V)**  


##  Analysis Approach

###  Data Preparation

- Dataset loaded and inspected  
- Verified no missing values  
- Selected relevant features for modeling  
- Split data into training (80%) and testing (20%)  


##  Simple Linear Regression

A simple linear regression model was built using:

- Input feature: **LSTAT (lower income population %)**
- Target: **House price**

###  Model Equation
MEDV = -0.9665 × LSTAT + 34.8369

###  Interpretation

- As the percentage of lower-income population increases → house prices decrease  
- Negative slope indicates an inverse relationship  

###  Model Performance

- MSE: **33.52**  
- R²: **0.54**  

 The model explains about **54% of the variance** in house prices   



###  Visualization

- Scatter plot shows a clear downward trend  
- Regression line fits overall pattern  
- Some data points scatter → prediction errors exist  



##  Multiple Linear Regression

To improve accuracy, additional important features were selected:

- ROOM  
- LSTAT  
- Student-teacher ratio  
- POLLUTION  

These features have strong relationships with house prices.



###  Model Performance (Improved)

- MSE: **26.98**  
- R²: **0.63**  

 The model now explains about **63% of price variation** 【1-e46aa9】  



###  Key Improvement

- Lower MSE → less prediction error  
- Higher R² → better explanation of data  



##  Key Insights

-  House prices decrease as lower-income percentage increases  
-  Number of rooms positively influences house prices  
-  Pollution and educational factors impact pricing  
-  Using multiple features significantly improves model performance  
-  Linear regression captures trends but cannot explain all variations  



##  Tools & Technologies

- Python  
- Pandas  
- Scikit-learn  
- Matplotlib  


##  Conclusion

This project demonstrates:

- The difference between simple and multiple regression  
- The importance of feature selection  
- How socioeconomic factors affect house prices  
- The role of evaluation metrics (MSE & R²)  

Multiple Linear Regression provided **better predictions** and reduced error compared to using a single feature.
