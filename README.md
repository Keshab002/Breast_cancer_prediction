# Breast Cancer Prediction Project

## Overview

This project focuses on predicting breast cancer using a dataset that includes 698 entries with various features related to cell characteristics. The goal is to build a predictive model using logistic regression, assess its performance through a confusion matrix, and finally, evaluate its accuracy using k-fold cross-validation.

## Dataset

The dataset contains 698 entries with the following columns:

1. **Clump Thickness**
2. **Uniformity of Cell Size**
3. **Uniformity of Cell Shape**
4. **Marginal Adhesion**
5. **Single Epithelial Cell Size**
6. **Bare Nuclei**
7. **Bland Chromatin**
8. **Normal Nucleoli**
9. **Mitoses**

## Data Cleaning

Data cleaning is a crucial step in preparing the dataset for modeling. In this project, the following data cleaning steps were performed:

- Handling missing values in any of the columns.
- Removing duplicate entries.
- Ensuring data types are appropriate for each column.
- Handling outliers or erroneous data points if necessary.

## Model Building - Logistic Regression

Logistic Regression is a popular choice for binary classification problems like breast cancer prediction. In this project, we have used logistic regression to build the predictive model.

## Confusion Matrix

A confusion matrix is a useful tool to evaluate the performance of a classification model. It provides insights into the number of true positives, true negatives, false positives, and false negatives. This project includes the creation and analysis of a confusion matrix to assess the model's ability to correctly classify cancer cases.

## Accuracy Evaluation - K-fold Cross-Validation

To ensure the robustness of the model and to prevent overfitting, k-fold cross-validation is employed to evaluate the model's accuracy. Cross-validation helps estimate the model's performance on unseen data by dividing the dataset into k subsets and training the model k times, each time using a different subset for validation. The average accuracy across all iterations is then calculated.

## How to Use

To replicate this project, follow these steps:

1. Obtain the breast cancer dataset with the specified columns: Clump Thickness, Uniformity of Cell Size, Uniformity of Cell Shape, Marginal Adhesion, Single Epithelial Cell Size, Bare Nuclei, Bland Chromatin, Normal Nucleoli, and Mitoses.

2. Perform data cleaning, including handling missing values, removing duplicates, and addressing outliers.

3. Implement logistic regression to build the predictive model.

4. Create a confusion matrix to assess model performance.

5. Perform k-fold cross-validation to evaluate model accuracy.

6. Analyze the results and fine-tune the model as needed.

7. Document your findings and share your insights with stakeholders or colleagues.

## Key Findings

### Confusion Matrix Analysis

Utilizing the `confusion_matrix` from the `sklearn.metrics` module, we examined the performance of our logistic regression model on a test set. The matrix revealed the following results:

|                  | Predicted Negative | Predicted Positive |
|------------------|--------------------|--------------------|
| Actual Negative  |         89         |          3         |
| Actual Positive  |          2         |         43         |

This matrix allowed us to analyze the model's ability to correctly classify instances, showcasing 89 true negatives, 43 true positives, 3 false positives, and 2 false negatives.

### Accuracy Calculation

The accuracy of our model on the test set was calculated using the `accuracy_score` function, yielding an accuracy of 96%. This metric provides an overall measure of the model's correctness in its predictions.

### K-Fold Cross-Validation

To further validate the model's robustness, we employed k-fold cross-validation with 10 folds. The accuracy scores obtained from each fold were averaged to provide a comprehensive assessment.

Average Accuracy: 96.70%
Standard Deviation: 2.28%

## Conclusion

In conclusion, the Breast Cancer Prediction Project successfully implemented a logistic regression model for accurate prediction of breast cancer based on cell characteristics. The confusion matrix and accuracy metrics demonstrated the model's commendable performance on the test set. The application of k-fold cross-validation further affirmed the model's consistency across various data subsets.

The project not only contributes to the field of medical diagnostics but also underscores the effectiveness of machine learning in predicting complex health conditions. Future iterations may explore additional features, algorithms, and optimization techniques to enhance predictive capabilities and extend the applicability of the model.
