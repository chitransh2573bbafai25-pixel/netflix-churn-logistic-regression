# netflix-churn-logistic-regression
Machine Learning practical using Logistic Regression to predict Netflix subscriber churn based on engagement, tenure, support, payment, and subscription plan data.
# Netflix Churn Prediction using Logistic Regression

This project uses **Logistic Regression** to predict whether a Netflix subscriber is likely to **churn (cancel their subscription)**.

The notebook uses a realistic **synthetic dataset** because Netflix's real subscriber data is private.

## Project Overview

The model analyzes subscriber information such as:

* Tenure in months
* Weekly watch hours
* Logins per month
* Support tickets
* Payment failures
* Subscription plan
* Churn status

The dataset contains **3,000 subscribers**, with churn represented as `1` and staying as `0`.

## Machine Learning Process

1. Create the synthetic subscriber dataset
2. Explore the data and churn rate
3. Convert subscription plans using one-hot encoding
4. Split data into 80% training and 20% testing
5. Scale the features
6. Train a Logistic Regression model
7. Evaluate predictions using accuracy and a confusion matrix
8. Analyze model coefficients
9. Predict churn probability for individual subscribers

## Model

**Algorithm:** Logistic Regression

The model assigns a coefficient to each feature. Positive weights increase churn risk, while negative weights push the prediction toward staying.

## Key Findings

The model identifies **payment failures and low engagement** as factors that increase churn risk, while **longer tenure and a Premium plan** reduce churn risk.

## Business Application

Subscribers identified as high-risk could be sent to a retention team for actions such as:

* Discount offers
* Free upgrade months
* Proactive customer support

This can help a streaming business identify customers who may cancel their subscriptions.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* Logistic Regression

## Important Note

This project is designed for a classroom case study and uses **synthetic data**. A real-world deployment would require actual subscriber data along with appropriate privacy and governance controls.
