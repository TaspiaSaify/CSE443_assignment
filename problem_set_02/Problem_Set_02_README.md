# Problem Set 02 - Bank Marketing Prediction Using Logistic Regression

## Overview
This project uses Logistic Regression to predict whether a customer will subscribe to a term deposit.

Target variable:
- No = 0
- Yes = 1

## Dataset
- Total records: 45,211
- Original features: 16
- Features after categorical encoding: 42
- Training data: 36,168
- Testing data: 9,043

## Approach
1. Loaded the Bank Marketing dataset.
2. Checked the dataset structure.
3. Checked for missing values.
4. Converted the target variable `y` into numerical values.
5. Separated features (X) and target (y).
6. Applied one-hot encoding to categorical variables.
7. Split the dataset into training and testing sets.
8. Applied StandardScaler for feature scaling.
9. Built a Logistic Regression model.
10. Trained the model using the training data.
11. Predicted values for the test data.
12. Evaluated the model using accuracy, classification report, and confusion matrix.

## Model
Machine learning algorithm used:
**Logistic Regression**

The model was trained with `max_iter=1000`.

## Results
The model achieved:
**Test Accuracy: 90.12%**

## Evaluation
The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Findings
The Logistic Regression model achieved approximately 90.12% test accuracy. However, the dataset contains many more "No" responses than "Yes" responses, so accuracy alone may not fully describe the model's performance.

## Conclusion
A Logistic Regression model was successfully developed for predicting term-deposit subscription. After preprocessing, categorical encoding, feature scaling, and model training, the model achieved 90.12% test accuracy.
