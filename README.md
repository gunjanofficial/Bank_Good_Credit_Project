# Bank_Good_Credit_Project
I have built the model where we can predict the bank customers credit card score based on the given features. With the help of credit score we can determine a customer’s credit worthiness and help the bank in reducing credit default risk. 
# Domain Analysis
dt_opened_x: This column likely represents the date when the credit card account or loan was opened for the customer. The "x" may imply that there are multiple similar columns related to the opening date of various financial products.

customer_no: This column contains a unique identifier or number assigned to each customer. It helps distinguish one customer from another in the dataset.

upload_dt_x: This column may indicate the date when this particular data entry or information was uploaded or recorded in the dataset.

acct_type: This column represents the type of account, such as credit card, personal loan, mortgage, etc. It specifies the financial product associated with the customer.

owner_indic: This column could be a binary indicator (1 or 0) that shows whether the account is owned by the customer (1) or not (0).

opened_dt: Similar to dt_opened_x, this column likely denotes the date when the account was initially opened.

last_paymt_dt: This column may indicate the date of the customer's last payment on the account.

reporting_dt: This column likely represents the date when the information about the account was reported to a credit bureau or data repository.

high_credit_amt: This column contains the highest credit amount ever extended to the customer for this account.

cur_balance_amt: This column represents the current outstanding balance on the account.

paymt_str_dt: This column may indicate the start date of a specific payment period.

paymt_end_dt: This column may indicate the end date of a specific payment period
    
dt_opened_y: This column likely represents the date when the credit card account or loan was opened for the customer. The "y" may imply that there are multiple similar columns related to the opening date of various financial products.

entry_time: This column may indicate the time or timestamp when the data entry was recorded or logged in the dataset.   
    
Bad_label: This column could be a binary indicator (1 or 0) that classifies whether the customer's credit behavior is considered bad (1) or good (0). It is likely the target variable used for credit risk prediction or classification modeling.

dt_opened: This column likely represents the date when the credit card account or loan was opened for the customer. It shows when the financial product was first established for the customer.

upload_dt_y: This column may indicate the date when this particular data entry or information was uploaded or recorded in the dataset. The "y" may suggest that there are multiple similar columns related to upload dates.

enquiry_dt: This column likely represents the date when an enquiry or credit inquiry was made for the customer. Credit inquiries occur when a lender or financial institution checks the customer's credit report to assess their creditworthiness for a new credit application.

enq_purpose: This column indicates the purpose of the credit inquiry made on the customer's credit report. It can include various reasons, such as credit card application, loan application, mortgage, etc.

enq_amt: This column represents the amount of credit requested or applied for during the credit inquiry. It shows the credit limit or loan amount the customer is seeking from the lender.    

# Data Analysis Report
This project belongs to the banking sector, where the objective is to build a model based on historical information. The goal is to predict customers' credit card scores, aiding the bank in mitigating credit default risk.

The dataset comprises three tables: Customers' Account, Customers' Demographics, and Customers' Enquiry. The Customers' Account table contains historical account and payment data. The Customers' Demographics table holds customers' personal details, with features anonymized according to privacy policies. Lastly, the Customers' Enquiry table contains historical inquiry data, including the inquiry amount and purpose.

Initially, I focused on comprehending the dataset's critical features for subsequent processes. As the dataset resided in a MySQL server, I installed necessary libraries, established a database connection, and extracted data into distinct variables. Upon merging the tables, I encountered a challenging dataset with 108 columns and around 4.9 million rows. I exported this data to a CSV file using Pandas.

Conducting basic checks unveiled foundational insights about the data. I observed substantial null values and categorical data in features, along with numerous unnecessary features. However, due to project constraints, in-depth exploratory data analysis was deferred.

During data preprocessing, I addressed null values, discarding features with over 50% null values, and dropped unnecessary columns. I employed mean, median, and mode imputation methods to fill missing values. Given categorical features, I applied label encoding for numerical conversion and adjusted specific datatypes using the astype function.

For exploratory data analysis (EDA), I focused on relevant features. Analyzing relationships between independent and dependent variables yielded valuable insights into customers' credit card behavior.

Feature selection involved exploring data correlations using a heatmap. Identifying highly correlated features, I dropped redundant ones. I standardized the dataset using the MinMaxScaler, established independent and dependent variables, and balanced the dataset using the SMOTE technique.

In the model creation phase, I employed logistic regression, decision tree classification, XGBoost classifier, artificial neural network (ANN) with MLP classifier, and random forest classifier. After training, I assessed models using accuracy, F1-score, precision, and classification reports. All models exhibited strong performance except for logistic regression classification. Notably, the random forest classifier achieved a remarkable 99.99% accuracy.

# Challenges faced during the Project¶
In this project, I encountered a large dataset with 108 columns and approximately 4.9 million rows after merging all the tables into a single variable. A significant amount of time was devoted to understanding the dataset and determining how to manage it effectively.

The dataset consisted of numerous columns, and it was crucial to possess domain knowledge about these features. This understanding enabled us to identify which features were essential for training the model and which could be dropped.

Many columns were labeled as 'feature1,' 'feature2,' and so on, making it challenging to comprehend their meanings. The dataset contained a substantial number of null values. Additionally, a majority of the features were categorical, contributing to class imbalance. To address these challenges, we employed statistical techniques and methodologies.

To gain insights, we performed exploratory data analysis (EDA) on a subset of features to observe their relationships. However, due to security concerns, a significant portion of features was concealed, limiting our ability to conduct comprehensive EDA."

# Conclusion of the project
We applied various algorithms to predict customers' bank credit card scores using historical data. Initially, we used five different algorithms and assessed their accuracy scores. Among them, decision tree classification and random forest classification showed exceptional performance, achieving an accuracy of 99.99%. This level of accuracy stands out when compared to the performance of other models.

Considering the remarkable performance of both decision tree classification and random forest classification, either of these algorithms could be considered the best choice for prediction. Both models exhibit a 99.99% accuracy rate, as shown in the comparison DataFrame."


                                                  _____________________________Done_________________________________
