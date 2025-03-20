# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to build and evaluate machine learning models to predict the likelihood of loans being classified as high-risk. The financial dataset contained information on loan status, with the target variable being the classification of loans as either "healthy" (0) or "high-risk" (1). Understanding these classifications is crucial for lenders to make informed decisions and mitigate financial risk.

The machine learning process involved several key stages: data preprocessing, model training, evaluation, and interpretation of results. Logistic Regression, XGBoost Classifier, K-Nearest Neighbors (KNN), and LightGBM (LGBM) were used as models to classify the loans due to their effectiveness in binary classification problems. The dataset was split into training and testing sets to ensure the models' performance could be evaluated on unseen data. Key metrics such as accuracy, precision, recall, F1-score, and AUC (Area Under the ROC Curve) were analyzed to assess model performance.

## Results

* Machine Learning Model: Logistic Regression

    * Training Results:

        * Accuracy: 99%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 0.99

        * Precision for High-Risk Loans (1): 0.85

        * Recall for High-Risk Loans (1): 0.98

        * AUC: 0.9942

    * Testing Results:

        * Accuracy: 99%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 1.00

        * Precision for High-Risk Loans (1): 0.88

        * Recall for High-Risk Loans (1): 0.98

        * AUC: 0.9970
    * Machine Learning Model: XGBoost Classifier

        * Training Results:

            * Accuracy: 99%

            * Precision for Healthy Loans (0): 1.00

            * Recall for Healthy Loans (0): 0.99

            * Precision for High-Risk Loans (1): 0.85

            * Recall for High-Risk Loans (1): 0.99

            * AUC: 0.9978

    * Testing Results:

        * Accuracy: 100%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 1.00

        * Precision for High-Risk Loans (1): 0.88

        * Recall for High-Risk Loans (1): 0.99

        * AUC: 0.9977

* Machine Learning Model: K-Nearest Neighbors (KNN)

    * Training Results:

        * Accuracy: 99%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 0.99

        * Precision for High-Risk Loans (1): 0.85

        * Recall for High-Risk Loans (1): 0.99

        * AUC: 0.9970

    * Testing Results:

        * Accuracy: 100%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 1.00

        * Precision for High-Risk Loans (1): 0.88

        * Recall for High-Risk Loans (1): 0.99

        * AUC: 0.9971

* Machine Learning Model: LightGBM (LGBM)

    * Training Results:

        * Accuracy: 99%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 0.99

        * Precision for High-Risk Loans (1): 0.85

        * Recall for High-Risk Loans (1): 0.99

        * AUC: 0.9982

    * Testing Results:

        * Accuracy: 100%

        * Precision for Healthy Loans (0): 1.00

        * Recall for Healthy Loans (0): 1.00

        * Precision for High-Risk Loans (1): 0.88

        * Recall for High-Risk Loans (1): 0.99

        * AUC: 0.9975

## Summary

All four models — Logistic Regression, XGBoost, K-Nearest Neighbors (KNN), and LightGBM (LGBM) — performed exceptionally well in predicting both healthy and high-risk loans. The AUC scores for all models exceeded 0.99, indicating strong discriminatory power between the two classes. Both Logistic Regression and KNN delivered similar performance, with AUC scores of 0.9942 and 0.9970, respectively. XGBoost and LGBM had slightly higher AUC scores of 0.9978 and 0.9982, making them marginally better performers.

In terms of precision and recall, all models achieved near-perfect scores for predicting healthy loans, with precision and recall values close to 1. For high-risk loans, all models maintained high recall scores of 98-99%, ensuring that the majority of high-risk loans were accurately identified. Precision for high-risk loans was slightly lower at 0.85 for training and 0.88 for testing, indicating occasional misclassification of healthy loans as high-risk.

Based on these results, the LightGBM model performed slightly better overall, with the highest AUC during training (0.9982) and strong recall for high-risk loans. XGBoost also performed exceptionally well, with slightly lower AUC scores but similar recall. Given the importance of identifying high-risk loans to minimize financial loss, LightGBM is recommended as the top choice. Further improvements could focus on increasing precision for high-risk loans to reduce false positives.
