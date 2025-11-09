# Project 3 — Building a Classifier using Titanic Dataset

## Objective
To use the titanic dataset to build and evaluate three classifiers: Decision Tree, Support Vector Machine and Neural Netowrk to compare model performance on predicting passenter survival. 

---

## Introduction


In this project, we use Titanic dataset which is a pre-loaded dataset that contains demographic and survival information for the passengers of the RMS Titanic. It includes features like passenger class, sex, age, fare and survival status. We use this titanic dataset to build and evaluate three classifier models: Decision Tree, Support Vector Machine and Neural Network to compare model performance on their effectiveness for predicting passenger survival. 

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

### Section 4: Train a Classifcation Model (Decision Tree)
1. Split the data
2. Create and Train Model (Decision Tree)
3. Predict and Evaluate Model performance
4. Report confusion matrix (as a heatmap)
5. Report Decision Tree plot
   
### Section 5: Compare Alternative Models (SVC, NN)
1. Train and Evaluate Model (SVC)
2. Visualize Support Vectors
3. Train and Evaluate Model (Neural Network on Case 3)
4. Visualize (Neural Network on Case 3)

### Summarize the findings
| Model Type           | Case   | Features Used     | Accuracy | Precision | Recall | F1-Score | Notes |
| -------------------- | ------ | ----------------- | -------- | --------- | ------ | -------- | ----- |
| Decision Tree        | Case 1 | alone             | 62.57%   | 51.28%    | 57.97% | 54.42%   | -     |
| Decision Tree        | Case 2 | age               | 61.45%   | 50.00%    | 17.39% | 25.81%   | -     |
| Decision Tree        | Case 3 | age + family_size | 59.22%   | 46.15%    | 34.78% | 39.67%   | -     |
| SVM (RBF Kernel)     | Case 1 | alone             | 62.57%   | 51.28%    | 57.97% | 54.42%   | -     |
| SVM (RBF Kernel)     | Case 2 | age               | 63.13%   | 71.43%    | 7.25%  | 13.16%   | -     |
| SVM (RBF Kernel)     | Case 3 | age + family_size | 63.13%   | 71.43%    | 7.25%  | 13.16%   | -     |
| Neural Network (MLP) | Case 3 | age + family_size | 65.36%   | 55.93%    | 47.83% | 51.56%   | -     |




   

---
