# Bank Customer Churn Prediction

## Objective

The goal of the **Bank Customer Churn Prediction** project is to identify customers who are at risk of leaving the bank. By predicting which customers are likely to churn, the bank can implement targeted strategies to retain these customers, thereby maintaining a stable customer base and minimizing revenue loss.

## Overview

### Data Visualization

Data visualization was performed using various charts to gain insights into customer behavior and the factors influencing churn. This step involved exploring relationships and patterns within the data to guide the predictive modeling process.

### Model Building

To predict customer churn, the following ensemble approach was adopted:

1. **Classifiers**:
   - **RandomForestClassifier**: An ensemble learning method that builds multiple decision trees and combines their outputs.
   - **XGBClassifier**: A gradient boosting algorithm known for its high performance and efficiency.


2. **Voting Classifier**:
   - A `VotingClassifier` was created to combine the predictions from both `RandomForestClassifier` and `XGBClassifier`.
   - **Voting Strategy**: Hard voting, where the final prediction is based on the majority vote among the classifiers.

### Training and Evaluation

- **Training**: The ensemble model was trained on the training dataset (`X_train` and `y_train`).
- **Evaluation**: The model’s performance was assessed using several metrics:
  - **Accuracy**: The proportion of correctly classified instances.
  - **Precision**: The proportion of true positive predictions among all positive predictions.
  - **Recall**: The proportion of true positive predictions among all actual positives.

### Predictions

After training the model, it was used to predict customer churn labels for the test dataset (`X_test`).

## Results

The ensemble model demonstrated robust performance in predicting customer churn, with notable metrics including accuracy, precision, and recall. The visualizations and metrics provided insights into the model's effectiveness and the factors influencing churn.


