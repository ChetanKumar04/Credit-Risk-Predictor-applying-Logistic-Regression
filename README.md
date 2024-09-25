**Credit Risk Classification Using Logistic Regression: A Data-Driven Approach**

This project leverages logistic regression to build a predictive model that classifies loan applicants based on credit risk. The goal is to accurately distinguish between low-risk (healthy) and high-risk loan applicants, using a set of key financial indicators. This model serves as a decision-making tool for lenders, helping to minimize loan defaults and optimize lending strategies.

**Objective**
The primary goal of this analysis is to create a model that can reliably predict whether an applicant falls into the ‘healthy loan’ or ‘high-risk loan’ category. The model is built using various financial factors, such as:

*Loan amount
*Interest rate
*Borrower’s income
*Debt-to-income ratio
*Number of existing accounts
*Predefined derogatory marks
*Total outstanding debt

The performance of the model will be evaluated in terms of its ability to accurately classify these categories, focusing on precision, recall, and overall accuracy.

**Methodology**
Two different models were developed and tested:

**Model 1: Original Data (Imbalanced Dataset)**

The dataset was initially imbalanced, consisting of approximately 97% healthy loans (75,036 records) and only 3% high-risk loans (2,500 records).
The data was split into training and testing sets, and a logistic regression model was trained on this imbalanced dataset.
Performance was assessed using confusion matrices, evaluating accuracy, precision, and recall.

**Model 2: Resampled Data (Balanced Dataset)**

To address the imbalance, the dataset was resampled, creating an equal number of healthy loans and high-risk loans (56,271 records for each category).
The logistic regression model was retrained on this balanced data, followed by the same evaluation using confusion matrices, precision, recall, and accuracy.

**Analysis Results**
Here’s how both models performed:

**Model 1 (Original Imbalanced Data)**

Balanced Accuracy: 99% on test data
Precision for Healthy Loans: 100%
Precision for High-Risk Loans: 85%
Recall for Healthy Loans: 99%
Recall for High-Risk Loans: 91%

**Model 2 (Resampled Balanced Data)**

Balanced Accuracy: 99% on test data
Precision for Healthy Loans: 99%
Precision for High-Risk Loans: 99%
Recall for Healthy Loans: 99%
Recall for High-Risk Loans: 99%

**Key Findings**

**Model 1 (Imbalanced Dataset):** 
While this model excelled at identifying healthy loans (with precision and recall near 100%), it struggled with classifying high-risk loans. The lower precision and recall for high-risk loans (85% precision, 91% recall) reflect the impact of the imbalanced dataset. The model tends to predict fewer high-risk loans accurately, which could lead to missed opportunities in risk mitigation for lenders.

**Model 2 (Resampled Dataset):** 
By balancing the dataset, the second model significantly improved its ability to classify high-risk loans. With precision and recall both reaching 99% for both loan categories, this model offers a far more consistent and accurate prediction, making it highly valuable for identifying risky applicants.

**Conclusion & Recommendations**

The second model, which uses the resampled dataset, outperforms the first model, especially in identifying high-risk loan applicants. This model is particularly valuable because of the high financial cost of misclassifying a high-risk loan as healthy, compared to the relatively low cost of misclassifying a healthy loan as risky. The ability to better identify high-risk applicants directly translates into reduced default rates and optimized lending strategies, making the resampled model the more effective choice for credit risk assessment.

This project illustrates the power of logistic regression in tackling real-world financial problems, especially when dataset imbalances are addressed. By resampling the data, we were able to improve predictive performance and deliver a more reliable tool for lenders.






