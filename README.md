# Customer-Churn-Prediction 

📌 Project Overview
Customer churn is a major challenge in the telecom industry. This project analyzes customer behavior for a telecom company Neo and builds machine learning models to predict whether a customer is likely to churn. The goal is to identify key drivers of churn and provide actionable business recommendations to improve customer retention.

🧾 Dataset Description
Dataset: customer_churn
Domain: Telecom
Target Variable: Churn (Yes / No)
Key Features Used:
tenure
MonthlyCharges
InternetService
Contract
PaymentMethod
SeniorCitizen
The dataset contains customer demographics, service usage, billing details, and churn information.

🔍 Exploratory Data Analysis (EDA)
The following analyses were performed:
Customer segmentation based on tenure, contract type, and payment method
Distribution Analysis of Internet Services
Tenure distribution using a histogram
Relationship between tenure and monthly charges using a scatter plot
Churn distribution analysis

Key observation:
The dataset is imbalanced, with a higher proportion of churned customers. Therefore, accuracy alone is not sufficient for model evaluation.

📊 Data Visualization
Bar Plot: Distribution of Internet Service categories
Histogram: Distribution of customer tenure
Scatter Plot: Tenure vs Monthly Charges
Box Plot: Tenure across different Contract types
These visualizations help understand customer behavior and service usage patterns.

🤖 Models Implemented
The following machine learning models were built and evaluated:
Linear Regression
Target: MonthlyCharges
Feature: tenure
Metric: RMSE
Logistic Regression
Simple Logistic: MonthlyCharges → Churn
Multiple Logistic: tenure + MonthlyCharges → Churn
Decision Tree Classifier
Feature: tenure
Target: Churn
Random Forest Classifier
Features: tenure, MonthlyCharges
Target: Churn

📈 Evaluation Metrics
For classification models, the following metrics were used:
Confusion Matrix
Accuracy Score
Classification Report (Precision, Recall, F1-score)
Recall is significant because failing to identify a churn customer can result in revenue loss.

🔑 Key Insights
Customers with low tenure are more likely to churn
Higher monthly charges increase churn probability
Long-term contracts significantly reduce churn
Tenure is the most influential feature in churn prediction (based on Random Forest feature importance)

💡 Business Recommendations
Focus retention campaigns on new customers
Offer discounts or personalized plans for high monthly charge customers
Promote long-term contracts to reduce churn risk
Use a churn prediction model to proactively engage at-risk customers

🛠 Tech Stack
Python
Pandas, NumPy
Matplotlib
Scikit-learn
Jupyter Notebook / Anaconda / Google Colab

🚀 Future Improvements

Handle class imbalance using SMOTE or class weights
Add more customer behavior features
Hyperparameter tuning using GridSearchCV
Deploy the model using Streamlit

👤 Author
Shital Pandey
Aspiring Data Scientist | Python & Machine Learning Enthusiast
