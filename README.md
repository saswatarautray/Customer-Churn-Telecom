# Customer-Churn
Telco customer data analysis: 
"Predict behavior to retain customers. You can analyze all relevant customer data and develop focused customer retention programs."

# Business Understanding
Machine learning enables decision makers to predict customer churn using company-owned historical data.

# Dataset

[IBM Sample Data Sets] https://www.kaggle.com/blastchar/telco-customer-churn 

Each row represents a customer, each column contains customer’s attributes described on the column Metadata. The raw data contains 7043 rows (customers) and 21 columns (features). The “Churn” column is our target.

### Data Dictionary

* customerID: Customer ID
* gender: Whether the customer is a male or a female
* SeniorCitizen: Whether the customer is a senior citizen or not (1, 0)
* Partner: Whether the customer has a partner or not (Yes, No)
* Dependents: Whether the customer has dependents or not (Yes, No)
* Tenure: Number of months the customer has stayed with the company
* PhoneService: Whether the customer has a phone service or not (Yes, No)
* MultipleLines: Whether the customer has multiple lines or not (Yes, No, No phone service)
* InternetService: Customer’s internet service provider (DSL, Fiber optic, No)
* OnlineSecurity: Whether the customer has online security or not (Yes, No, No internet service)
* OnlineBackup: Whether the customer has an online backup or not (Yes, No, No internet service)
* DeviceProtection: Whether the customer has the device protection or not (Yes, No, No internet service)
* TechSupport: Whether the customer has the tech support or not (Yes, No, No internet service)
* StreamingTV: Whether the customer has TV streaming or not (Yes, No, No internet service)
* StreamingMovies: Whether the customer has movie streaming or not (Yes, No, No internet service)
* Contract: The customer’s contract 
* PaperlessBilling: Whether the customer has paperless billing or not (Yes, No)
* PaymentMethod: The payment method opted by the customers 
* MothlyCharges: The monthly charges paid by the customers
* TotalCharges: The total charges paid by the customers
* Churn: The customer churn status (1 - Yes, 0 - No)

# Data preparation 

### -Code Used:
* Python Version : 3.7.6
* Packages : Pandas, Numpy, Sklearn, Matplotlib, Seaborn

### -Inspect The Initial Condition of Data

# Data Cleansing
* Missing Values Checking and Handling
* Duplicates Checking
* Anomali and Outlier Detection
* Data Type Correction
* Feature Extraction

# Exploratory Data Analysis
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables.

![image](https://user-images.githubusercontent.com/75175081/122672328-4503c600-d1f5-11eb-8ebc-527c48a06abf.png)
![image](https://user-images.githubusercontent.com/75175081/122672333-4a611080-d1f5-11eb-8c1f-3a8b2666596c.png)

# Modeling
* Split the data into train and tests sets with a test size of 25%.
* I tried three different models: Support vector machine, Decision Tree Model, and Random Forest Model.
* Evaluated them using AUC (Area Under ROC Curve). 
* I chose AUC because it is relatively easy to interpret model performance.

# Evaluation
* The evaluation metric that be used is AUC (Area Under ROC Curve).
* The Random Forest model has better performence than the other approaches on the test and validation sets.

![image](https://user-images.githubusercontent.com/75175081/122672450-be031d80-d1f5-11eb-94a1-f25e99a2cf18.png)

# Summary
* Machine learning enables decision makers to predict customer churn using company-owned historical data.
* The evaluation metric that be used is AUC (Area Under ROC Curve).
* Tried three different models: Support vector machine, Decision Tree Model, and Random Forest Model.
* The Random Forest model has better performence than the other approaches on the test and validation sets.

