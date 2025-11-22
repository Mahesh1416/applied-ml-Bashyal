# Project 5 — Ensemble Machine learning using wine dataset
---

## Introduction

In this project,we will use wine quality dataset to compare two ensemble models to evaluate their model performance. We will compare two models, Bagging and MLP classifier model based on accuracy and F1 scores to predict which will perform better with this dataset. 
___

## Steps Involved

### Section 1: Load and Inspect the data
1. Import necessary libraries  
2. Load the wine dataset 
3. Display basic dataset information  
---

### Section 2: Prepare the data
---

### Section 3: Feature Selection and Justification
1. Define input features and target
---
### Section 4: Split the Data into Train and Test
___

### Section 5: Evaluate Model Performance
| Option | Model Name                        | Notes                                                          |
| ------ | --------------------------------- | -------------------------------------------------------------- |
| 1      | Random Forest (100)               | A strong baseline model using 100 decision trees.              |
| 2      | Random Forest (200, max_depth=10) | Adds more trees, but limits tree depth to reduce overfitting.  |
| 3      | AdaBoost (100)                    | Boosting method that focuses on correcting previous errors.    |
| 4      | AdaBoost (200, lr=0.5)            | More iterations and slower learning for better generalization. |
| 5      | Gradient Boosting (100)           | Boosting approach using gradient descent.                      |
| 6      | Voting (DT + SVM + NN)            | Combines diverse models by averaging their predictions.        |
| 7      | Voting (RF + LR + KNN)            | Another mix of different model types.                          |
| 8      | Bagging (DT, 100)                 | Builds many trees in parallel on different samples.            |
| 9      | MLP Classifier                    | A basic neural network with one hidden layer.                  |

___

### Section 6. Compare Results

| Model               | Train Accuracy | Test Accuracy | Train F1  | Test F1  |
|--------------------|----------------|---------------|-----------|----------|
| MLP Classifier      | 0.851446       | 0.843750      | 0.814145  | 0.807318 |
| Bagging (DT, 100)   | 1.000000       | 0.884375      | 1.000000  | 0.865452 |



___

### Section 7. Conclusions and Insights

### Based on the results from the confusion matrix for the Bagging Model,this model is strong when identifying "medium cases" but poor in identifying "low cases" and better at identifying high quality wines compared to MLP model. 

### Similarly, based on the results from the confusion matrix for the MLP classified model, it is very strong when identifying "medium cases" and also similarly poor in identifying "low cases" but lower in identifying high quality wines compared to Bagging model.

### Based on metrics such as accuracy and F1 scores, Bagging method has better accuracy (0.88 vs 0.84) and slightly better F1 scores (0.86 vs 0.80) when compared to MLP classifier model. However, we also have to acknowledge the fact that there seems to be a little bit of overfitting problem with Bagging method as the gap between training and testing accuracy and F1 scores seems to be higher compared to MLP classifier method. 


### When I compared my results with the peers I found that Random Forest seems to do well based on accuracy and F1 scores while acknowledging that it may also have an overfitting problem. 

https://github.com/brandonjbbb/applied-ml-brandon/blob/main/notebooks/project05/ensemble-brandon.ipynb

### One of our colleague also found out that the boosting model such as (Adaboost) showed least performance values in accuracy and F1 score but had very small gaps between training and testing indicating stable generalization but limited capacity for this dataset.

https://github.com/wkarto/applied-ml-karto/blob/main/notebooks/project05/ensemble-karto.ipynb



---


