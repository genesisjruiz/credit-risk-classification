## Module 20: Supervised Learning
## Credit Risk Classification

### Overview of the Analysis

The purpose of this analysis was to build a machine learning model to predict loan status. The data used for this analysis was lending data, and the target variable to predict was `loan_status`. The `loan_status` variable is binary, indicating whether a loan is healthy (0) or high-risk (1). 

The machine learning process involved several stages:
1. Data was first loaded into a Pandas DataFrame.
2. The target variable `loan_status` was separated from the feature variables.
3. The data was split into training and testing sets.
4. A logistic regression model was trained on the training data.
5. The trained model was then used to make predictions on the testing data.

### Results

The logistic regression model's performance was evaluated using accuracy, precision, and recall scores. Here are the results:
**Logistic Regression Model Performance:**

* **Accuracy:** 0.99
* **Healthy Loans (0):**
  * **Precision:** 1.00
  * **Recall:** 0.99
  * **F1-Score:** 1.00
* **High-Risk Loans (1):**
  * **Precision:** 0.85
  * **Recall:** 0.91
  * **F1-Score:** 0.88
* **Overall:**
  * **Macro Average F1-Score:** 0.94
  * **Weighted Average F1-Score:** 0.99

### Summary

The logistic regression model performed quite well in predicting both healthy and high-risk loans. It had a high accuracy score of 0.99, indicating that it correctly predicted the loan status for 99% of the samples. 

The model had a high precision and recall for predicting healthy loans, meaning it was very effective at identifying true positives and limiting false positives for this class. For high-risk loans, the precision was slightly lower, but the recall was still high, indicating that the model was able to correctly identify a high percentage of the high-risk loans.

I would recommend the use of this model for loan status. However, depending on the risk tolerance of the lender, I would use additional models to mitigate the potential impacts of false negatives (a high-risk loan incorrectly predicted as healthy). 
