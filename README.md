
# MS634ProjD4: Advanced Data Mining for Healthcare and Socioeconomic Data

## Project Overview
This project applies advanced data mining and machine learning techniques to a large, real-world healthcare dataset. The goal is to extract actionable insights, build predictive models, and discover patterns relevant to healthcare and socioeconomic outcomes. Additional analyses use the UCI Adult Income dataset and the Diabetes dataset from `sklearn.datasets` for classification and regression modeling.

## Dataset Summary
The primary dataset (`healthcare_deliverable1.csv`) contains 55,500 records with the following features:
- **Demographics:** Name, Age, Gender, Blood Type
- **Medical:** Medical Condition, Date of Admission, Doctor, Hospital, Medication, Test Results
- **Administrative:** Insurance Provider, Billing Amount, Room Number, Admission Type, Discharge Date

## Project Steps
1. **Data Exploration & Cleaning:**
   - Loaded and explored the healthcare dataset.
   - Handled missing values (e.g., imputed median for missing ages).
   - Removed duplicate records to ensure data integrity.
   - Encoded categorical variables for modeling.

2. **Regression Modeling:**
   - Applied Linear, Ridge, and Lasso Regression to predict continuous outcomes (e.g., billing amount, diabetes progression).
   - Used cross-validation to assess model generalization.
   - Ridge Regression provided the best balance of bias and variance.

3. **Classification Modeling:**
   - Used Decision Tree, Naive Bayes, and K-Nearest Neighbors to classify outcomes (e.g., income >50K, medical conditions).
   - Performed hyperparameter tuning (GridSearchCV) for optimal Decision Tree performance.
   - Achieved accuracy of ~86% and F1 score of ~0.70 on test data.

4. **Clustering:**
   - Applied K-Means clustering to segment individuals into groups based on demographics and medical features.
   - Used PCA for visualization of clusters.

5. **Association Rule Mining:**
   - Used the Apriori algorithm to find frequent itemsets and generate association rules (e.g., between education, workclass, and income).

## Major Findings
- **Regression:**
  - Ridge Regression improved generalization and stability over plain Linear Regression.
  - Lasso Regression aided in feature selection but performed slightly worse.

- **Classification:**
  - Decision Tree with tuned hyperparameters achieved high accuracy and F1 score.
  - Most important features for income prediction included education and workclass.

- **Clustering:**
  - K-Means identified two main groups: one with lower education/income, another with higher education/income.

- **Association Rules:**
  - People with income >50K are strongly associated with having a Bachelor's degree and working in the private sector.
  - Those with a Bachelor's degree always had income >50K in the sample (100% confidence).

## Real-World Implications
- Insights can inform healthcare policy, targeted interventions, and resource allocation.
- Association rules can guide marketing, HR, and financial decision-making.


MSCS 634 – Project Deliverable 4
