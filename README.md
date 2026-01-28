# TripleTen-Sprint-17-Final-Project
📶 Final Project: Customer Churn Prediction — Interconnect Telecom
📝 Project Overview

Interconnect, a telecom operator, wants to forecast customer churn to proactively retain clients. By predicting which users are likely to leave, the company can offer promotional codes, plan upgrades, or special services to reduce churn.

This project involves merging multiple datasets, performing feature engineering, and building predictive models to estimate churn probability. The main goal is to maximize AUC-ROC, with Accuracy as an additional metric.

📊 Company Services

Interconnect provides:

Primary Services

Landline communication — multiple lines supported

Internet — DSL or fiber optic connections

Additional Services

Internet security: antivirus (DeviceProtection) and malicious website blocker (OnlineSecurity)

Dedicated technical support (TechSupport)

Cloud storage and backup (OnlineBackup)

TV streaming (StreamingTV) and movie directory (StreamingMovies)

Clients may choose monthly, 1-year, or 2-year contracts and multiple payment methods, receiving electronic invoices for transactions.

📊 Dataset Description

The dataset is composed of multiple files, each containing unique customer information:

File	Description
contract.csv	Contract information valid as of February 1, 2020
personal.csv	Client personal data
internet.csv	Internet service usage
phone.csv	Telephone service usage

All files contain the customerID column as a unique identifier.

Target feature: EndDate = 'No' (indicating churn).

Primary metric: AUC-ROC, secondary metric: Accuracy.

Dataset location: /datasets/final_provider/

Download link: Dataset

🎯 Objectives

Load and merge multiple datasets using customerID as a key

Explore and preprocess data (handle missing values, encode categorical variables, scale numerical features)

Engineer new features that improve predictive performance

Train and compare multiple classification models:

Logistic Regression

Decision Tree

Random Forest

Gradient Boosting (LightGBM, CatBoost, XGBoost)

Tune hyperparameters for optimal performance

Evaluate models using AUC-ROC and Accuracy

Select the best model for deployment to forecast churn

🔍 Key Tasks Performed
🧹 Data Preparation

Loaded and merged all source files (contract.csv, personal.csv, internet.csv, phone.csv)

Checked for missing and inconsistent values

Encoded categorical variables (e.g., contract type, payment method)

Normalized numerical variables (e.g., tenure, monthly charges)

📈 Exploratory Data Analysis

Analyzed churn distribution and key influencing features

Visualized correlations between service usage and churn

Identified high-risk segments for proactive retention strategies

🔧 Model Development

Trained multiple classification models using training and validation splits

Applied cross-validation to ensure model generalization

Tuned hyperparameters using grid search and randomized search

Selected the best model based on AUC-ROC and Accuracy metrics

📊 Model Evaluation

Primary evaluation metric: AUC-ROC

Secondary metric: Accuracy

Performance thresholds for assessment:

AUC-ROC	Points (SP)
< 0.75	0
0.75 – 0.81	4
0.81 – 0.85	4.5
0.85 – 0.87	5
0.87 – 0.88	5.5
≥ 0.88	6

Analyzed feature importance to understand key drivers of churn

🛠️ Tools & Technologies

Python

Pandas & NumPy for data processing

Scikit-learn for modeling and evaluation

LightGBM, XGBoost, CatBoost for gradient boosting models

Matplotlib & Seaborn for visualization

Jupyter Notebook

📈 Final Deliverables

Merged and cleaned dataset ready for modeling

Feature-engineered dataset with categorical and numerical preprocessing

Multiple classification models with hyperparameter tuning

Model evaluation using AUC-ROC and Accuracy

Feature importance analysis to guide retention strategies

Recommendations for proactive churn reduction

✅ Success Criteria

Accurate churn prediction with high AUC-ROC

Proper handling of multiple datasets and missing data

Clear comparison and selection of models based on performance

Documented feature engineering and workflow

Reproducible and clean code suitable for deployment

📌 Conclusion

This project demonstrates the application of machine learning to predict customer churn in telecom. By merging datasets, preprocessing features, and training multiple classification models, Interconnect can identify clients at risk of leaving and implement targeted retention strategies, ultimately improving revenue and customer satisfaction.
