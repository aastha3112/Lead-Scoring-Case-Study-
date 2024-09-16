# Lead-Scoring-Case-Study-

## Problem Statement

X Education markets online courses to industry professionals. The company acquires leads from website visitors, search engines, and referrals. The current lead conversion rate is low, with only 30% of leads converting into customers. To improve efficiency, the goal is to identify 'Hot Leads'—those with higher conversion potential—so the sales team can focus on them and enhance overall conversion rates.

## Steps Followed

### Data Collection
- Collected a dataset containing dependent (binary/categorical outcome) and independent variables (features/predictors).

### Data Preprocessing
- Handled missing values.
- Converted categorical variables to dummy variables (one-hot encoding).
- Normalized or scaled numerical features as needed.
- Split the data into training and testing sets.

### Model Building
- Imported necessary libraries such as `sklearn` and `statsmodels`.
- Initialized the logistic regression model.

### Training the Model
- Fitted the logistic regression model to the training data to learn the relationships between independent variables and the outcome variable.

### Model Evaluation
- Predicted probabilities and classes for the testing set.
- Evaluated the model using performance metrics: accuracy, precision, recall, F1-score, and ROC-AUC.

## Observations

1. ROC Curve of Training Data
   - AUC of 0.86 indicates strong performance in separating positive and negative classes. The model performs significantly better than random chance but has room for improvement.

2. Accuracy, Specificity, and Sensitivity of Training Data
   - Sensitivity: 78.71% (correct identification of positive cases).
   - Specificity: 78.69% (correct identification of negative cases).
   - Accuracy: 78.69% (overall correctness of predictions). Accuracy alone may not fully reflect model performance, especially with class imbalance.

3. Precision and Recall of Training Data
   - Precision: 69.47% (correct positive predictions).
   - Recall: 78.71% (correct identification of actual positive cases).
   - A trade-off is observed between precision and recall, with moderate accuracy in predicting positives but some true positives still missed.

4. ROC Curve of Test Data
   - AUC of 0.86 suggests good discrimination ability between classes, though there is room for further improvement.

5. Accuracy, Specificity, and Sensitivity of Test Data
   - Sensitivity: 79.27% (identification of positive cases).
   - Specificity: 77.04% (identification of negative cases).
   - Accuracy: 77.92% (overall prediction correctness). Sensitivity and specificity provide additional clarity beyond accuracy.

6. Precision and Recall of Test Data
   - Precision: 50.44% (correct positive predictions).
   - Recall: 62.31% (correct identification of actual positive cases).
   - A trade-off between precision and recall is evident, where improvements in one metric affect the other.

## Conclusion

- The model demonstrates strong performance with an AUC of 0.86, indicating good class discrimination. However, there is potential for improvement in accuracy and classification.
- Accuracy, sensitivity, and specificity are relatively consistent between training and test data, but a trade-off between precision and recall exists. Training data shows higher precision, while test data has higher recall.
- To optimize performance, focusing on balancing precision and recall is crucial. Techniques such as feature selection, model tuning, and cross-validation can enhance prediction reliability and generalization.
- Continued model refinement and evaluation will help address trade-offs and improve overall predictive accuracy, leading to more effective outcomes.

## Future Work

- Explore advanced techniques for better precision-recall balance.
- Implement cross-validation to ensure model robustness.
- Investigate additional features or models to improve performance.

