
# Customer Churn Prediction & Customer Retention Analysis

## 📌 Project Overview

Customer churn is a major business challenge for subscription-based businesses. Identifying customers who are likely to leave can help companies take proactive retention actions.

This project analyzes customer churn patterns using **Python, SQL, and Machine Learning**. The analysis first identifies important churn drivers and customer segments and then builds simple classification models to predict customers who may churn.

The project follows an end-to-end analytics approach:

**Data Cleaning → Exploratory Data Analysis → Business Analysis → SQL → Churn Prediction → Model Evaluation → Business Recommendations**

---

## 🎯 Business Objective

The key objectives of this project are to:

* Understand the overall customer churn rate.
* Identify customer segments with higher churn.
* Analyze factors associated with customer churn.
* Use SQL to answer business questions.
* Build simple classification models to predict churn.
* Identify high-risk customers for targeted retention efforts.
* Provide actionable business recommendations.

---

## 🗂️ Dataset

The dataset contains **1 million customer records** with customer demographic, contract, financial, service, satisfaction, and churn-related information.

Key variables include:

* Customer ID
* Age
* Gender
* Education
* Marital Status
* Contract Type
* Payment Method
* Monthly Charges
* Total Charges
* Customer Satisfaction
* Number of Service Calls
* Number of Complaints
* Late Payments
* Technical Support
* Churn

---

## 🛠️ Tools & Technologies

| Tool             | Purpose                               |
| ---------------- | ------------------------------------- |
| Python           | Data cleaning, EDA & Machine Learning |
| Pandas           | Data manipulation                     |
| NumPy            | Numerical operations                  |
| Matplotlib       | Data visualization                    |
| Seaborn          | Statistical visualizations            |
| SQL              | Business analysis                     |
| Scikit-learn     | Classification models                 |
| Jupyter Notebook | Project development                   |

---

# 🔍 Project Workflow

## 1. Data Cleaning & Validation

The raw dataset was inspected for:

* Missing values
* Duplicate records
* Incorrect data types
* Invalid values
* Inconsistent categories

Missing numerical values were handled using appropriate median-based imputation, while categorical and numerical columns were prepared for analysis.

---

# 2. Exploratory Data Analysis

EDA was performed to understand:

* Overall churn distribution
* Churn by contract type
* Churn by customer satisfaction
* Churn by payment behaviour
* Churn by service interactions
* Churn by complaints
* Churn by customer value
* Customer risk segments

### Key EDA Findings

* Overall customer churn rate is **9.92%**.
* Month-to-month customers have the highest churn rate at **26.51%**.
* Two-year contract customers have the lowest churn rate at **5.65%**.
* Customers with late payments and high service calls have a churn rate of **18.06%**.
* Month-to-month customers who are Detractors have the highest observed churn rate at **33.78%**.

These findings indicate that **contract type, customer satisfaction, payment behaviour, and service interactions** are important areas for retention efforts.

---

# 3. SQL Business Analysis

SQL was used to answer business-focused questions and identify important customer segments.

The analysis covered areas such as:

* Overall churn
* Churn by contract
* Churn by customer satisfaction
* Customer complaints
* Service calls
* Late-payment behaviour
* Customer risk groups
* Customer segmentation
* Churn patterns across different customer characteristics

The SQL analysis helped convert the raw customer data into actionable business insights.

---

# 4. Customer Churn Prediction

A classification approach was used to predict whether a customer is likely to churn.

Since the dataset contains 1 million records, a **200,000-row stratified sample** was used for the Machine Learning section to keep the notebook efficient and memory-friendly.

Two simple classification models were used:

### Logistic Regression

Used as a baseline classification model for predicting the binary churn outcome.

### Random Forest

Used to capture non-linear relationships between customer characteristics and churn.

---

# 5. Model Evaluation

The models were evaluated using:

* Accuracy
* Recall
* ROC-AUC

| Model               | Accuracy |    Recall | ROC-AUC |
| ------------------- | -------: | --------: | ------: |
| Logistic Regression |    63.3% |     63.7% |   0.684 |
| Random Forest       |    62.8% | **66.9%** |   0.680 |

### Model Interpretation

Logistic Regression achieved slightly higher **Accuracy and ROC-AUC**, while Random Forest achieved higher **Recall**.

Since identifying potential churners is important for customer retention, recall is particularly useful because it measures how many actual churners are successfully identified by the model.

The models provide useful churn-risk signals, but they should be used as a **customer prioritization tool rather than a perfect prediction system**.

---

# 📊 Important Churn Drivers

The Random Forest model identified several important features associated with churn prediction, including:

* Contract type
* Customer satisfaction
* Number of complaints
* Number of service calls
* Late payments
* Technical support
* Monthly charges
* Total charges

The ML findings are consistent with several patterns identified during the EDA and SQL analysis.

---

# 🎯 Customer Risk Identification

The churn model was also used to calculate the probability of churn for customers.

Customers can then be grouped into different risk levels:

* **Low Risk**
* **Medium Risk**
* **High Risk**

This provides a practical way for a business to prioritize customers who may require retention interventions.

Instead of targeting every customer, retention teams can focus more attention on customers with higher predicted churn risk.

---

# 💡 Key Business Recommendations

### 1. Encourage Longer-Term Contracts

Month-to-month customers have significantly higher churn than customers on longer contracts.

**Recommendation:** Introduce incentives, loyalty benefits, or special offers to encourage longer-term contracts.

### 2. Prioritize Dissatisfied Customers

Customers with lower satisfaction show higher churn risk.

**Recommendation:** Use proactive customer support and service-recovery initiatives for dissatisfied customers.

### 3. Monitor Service Issues

Repeated service calls and complaints are important churn signals.

**Recommendation:** Identify customers with repeated service interactions and provide proactive support before dissatisfaction increases.

### 4. Focus on High-Risk Segments

Customers combining multiple risk factors should receive higher priority.

**Recommendation:** Create targeted retention campaigns using both business rules and predicted churn probability.

---

# 📈 Business Impact

The analysis provides a framework for moving from **reactive churn management to proactive customer retention**.

A business can use the findings to:

* Identify high-risk customer segments.
* Prioritize retention campaigns.
* Improve customer service.
* Encourage longer-term contracts.
* Monitor dissatisfaction and service issues.
* Use predictive scores to support retention decisions.

---

# 📁 Project Structure

```text
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction.ipynb
├── README.md
└── customer_churn_dataset_10000.csv
```

---

# 🚀 Key Takeaway

The project combines **descriptive, diagnostic, and predictive analytics** to understand customer churn.

The analysis shows that **contract type, customer satisfaction, complaints, service interactions, and payment behaviour** are important areas to consider when managing churn.

Machine Learning further supports the analysis by identifying customers who may be at higher risk of churn, allowing businesses to prioritize retention efforts.

---

## 👩‍💻 Skills Demonstrated

**Python | Pandas | NumPy | SQL | Seaborn | Matplotlib | Exploratory Data Analysis | Feature Preparation | Logistic Regression | Random Forest | Classification | Model Evaluation | Business Analytics | Customer Segmentation | Data Visualization**
