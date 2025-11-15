# Project 4 — Continuous Target Prediction Using Regression In Titanic Data
---

## Introduction

In this project,we will use regression in order to predict a continuous numeric target. In other words, we will be predicting the fare of the Titanic using different features that are provided in this Titanic dataset.
___

## Steps Involved

### Section 1: Importing and Inspecting the data
1. Import necessary libraries  
2. Load the Titanic dataset  
3. Display basic dataset information  
---

### Section 2: Data Exploration and Preparation
1. Handle Missing Values and Clean Data
2. Create a new feature 
3. Perform feature engineering  

---

### Section 3: Feature Selection and Justification
1. Choose features and target 
2. Define **X** (features) and **y** (target) 

---

### Section 4: Train a Regression Model
1. Split the data
2. Train and Evaluate Linear Regression Models (all 4 cases)
3. Report performance
___

### Section 5: Compare Alternative Model
1. Ridge Regression (L2 Penalty)
2. Elastic Net (L1 + L2 combined)
3. Polynomial Regression
4. Visualize Polynomial Cubic Fit (for 1 input feature)
5. Compare all models
6. Visualize Higher Order Polynomial (for teh same 1 input case)

___

### Section 6. Final Thoughts and Insights
1. Summarize Findings
   

### Summarize the findings
| Model         | R²    | RMSE   | MAE    |
|---------------|-------|--------|--------|
| Linear        | 0.302 | 31.79  | 20.65  |
| Ridge         | 0.302 | 31.77  | 20.64  |
| ElasticNet    | 0.339 | 30.92  | 19.93  |
| Polynomial    | 0.336 | 30.99  | 19.25  |

___

2. Final Thoughts and Insights

### Section 6. Final Thoughts and Insights

- What features were most useful? We compared different features such as age, family size, age + family size and pclass to predict the fare. I found out the pClass was the best predictor for fate. 

- What regression model performed best? Based on R2 and other metrics, Elastic Net and Poynomial regression seem to do a better job than regular regression. 

- How did model complexity or regularization affect results? I noticed that initially the R squared values for Case 1 (age), family size, age + family size were very low, but for our fourth case (pClass), the R squared value was much better. This also helped with the underfitting which was observed in those initial cases. This tells us that it is very important to explore which feature works best as a predictor by using these metrics to improve the model. When I used the Elastic Net and Ridge models for pClass feature,slight improvmeent in R squared values were observed indicating better prediction than the linear models. 

   

---

