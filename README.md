# Cost-Sensitive-Spam-Email-Classification

## Overview
This GitHub project focuses on building and evaluating machine learning models for detecting spam messages using the Spambase dataset. The dataset, comprising 4601 email records with 58 attributes, is obtained from UCI Machine Learning Repository. (http://archive.ics.uci.edu/ml/machine-learning-databases/spambase/spambase.data)

## Project Structure
1. Data Preparation Download and Load Data: The Spambase dataset is downloaded from the provided URL. The data is loaded from the "spambase.data" file into a Pandas DataFrame. Handle Missing Values: Check for missing values and address them if necessary.

2. Exploratory Data Analysis (EDA): Explore the dataset to understand its structure, distribution, and features.

3. Data Preprocessing: Normalization: Use StandardScaler() to normalize the feature data, especially important for models like K-Nearest Neighbors (KNN).

4. Model Building: Classification Models: Build multiple classification models, including Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree, Random Forest, XGBoost, Support Vector Machine (SVM), and Neural Network.

5. Hyperparameter Tuning: Random Search, Perform hyperparameter tuning for each model using random search to optimize parameters and achieve the best performance.

6. Cross-Validation: Nested Cross-Validation: Implement nested cross-validation for model selection and evaluation. This includes an inner loop for hyperparameter tuning and an outer loop for assessing the models' performance.

7. Cost-Sensitive Modeling Cost Ratio: Set a 10:1 cost ratio for different misclassification errors, with a focus on minimizing false negatives (spam emails classified as non-spam).

8. Evaluation Metrics: Calculate various performance metrics for each model, including Accuracy, Precision, Recall, F1 Score, Area Under the Receiver Operating Characteristic (ROC-AUC), and Average Misclassification Cost.
9. Visualization: Create visualizations, such as ROC curves, to illustrate the performance of different models.

## Results
|Model| Accuracy |Precision | Recall |F1 Score |AUC-ROC |Avg. Misclassification Cost|
|-----|----------|----------|--------|---------|--------|---------------------------|
|Decision Tree	|0.91	|0.89|	0.88	|0.88| 0.90	 | 0.55 |
|KNN |0.90|	0.89|	0.86|	0.88|	0.90|	0.46|
|Logistic Regression|	0.93|	0.92|	0.89|	0.90|	0.92|	0.35|
|Random Forest|	0.95|	0.95|	0.92|	0.94|	0.95|	0.30|
|XG Boost|	0.95|	0.95|	0.93|	0.94|	0.95|	0.21|
|SVM|	0.93|	0.93|	0.89|	0.91|	0.93|	0.30|
|Neural Network|	0.94|	0.93|	0.92|	0.93|	0.94|	0.25|

## Conclusion
This project demonstrates the process of building, tuning, and evaluating machine learning models for spam detection using the Spambase dataset. The models' average performance metrics are presented, providing insights into their effectiveness in classifying spam and non-spam emails. Users can refer to this README for a comprehensive understanding of the project structure, methodology, and results.
