# UWML_frauddetection
Fraud detection from kaggle data


Project Description:
In present times, increased number of transaction frauds has enhanced need for fraud detection and prevention systems. Transaction fraud detection is now known as critical process for identification and prevention of fraudulent activities in financial transactions. This process involves use of advanced ML algorithms, data analytics, analysis of transaction patterns, and anomalies in transaction data. Using these advanced approaches, various parameters such as location, transaction amount, and frequency can be monitored to detect any unusual behaviour indicating frauds. Real-time monitoring and adaptive algorithms contribute to the effectiveness of fraud detection, enabling swift intervention to prevent unauthorized transactions and protect both consumers and financial institutions from potential losses.

Our approach:  
__________________________________
Dataset
Dataset used in this project was provided by Vesta Corporation in 2019 for a compeition on Kaggle.com. It contains real-time transaction details such as user details (device type, OS system), location, transaction amount, and other above 300 features for each transaction. The whole data set is broken into two files: identity and transaction files. These files are mergered using Transaction ID. 



Dataset Description

The dataset comes from the [IEEE-CIS Fraud Detection competition on Kaggle](https://www.kaggle.com/competitions/ieee-fraud-detection), hosted by Vesta Corporation in 2019. It includes over 300 anonymized features capturing transactional and identity attributes.

- `train_transaction.csv`: Contains information on each transaction (amount, time, product, card details, etc.)
- `train_identity.csv`: Includes additional information such as device type, browser, operating system, etc.
- Both datasets are merged using `TransactionID`.

### Example Features

- `TransactionDT`: Time delta
- `TransactionAMT`: Amount paid
- `ProductCD`: Product type
- `card1`–`card6`: Card and bank identifiers
- `addr1`, `dist1`: Location indicators
- `V1`–`V339`: Rich anonymized features engineered by Vesta

---

# Methodology

 **Data Cleaning & Merging**  
  Combined and cleaned the transaction and identity datasets, handled missing values, and created a unified dataset for training.

 **EDA (Exploratory Data Analysis)**  
  Visualized distributions of key variables, compared fraudulent vs. non-fraudulent samples, and assessed data imbalance.

 **Feature Engineering**  
  Applied encoding, transformations, and created new synthetic features to improve model performance.

**Modeling**  
  Trained and evaluated the following models:
  - Logistic Regression
  - Random Forest
  - Decision Tree

-  **Evaluation Metrics**  
  Focused on ROC-AUC score, Precision, Recall, F1-score, and confusion matrices for performance evaluation.

---

 Results Summary

| Model             | ROC-AUC | Precision | Recall |
|------------------|---------|-----------|--------|
| Logistic Regression | ~0.76   | ~0.65     | ~0.55  |
| Random Forest       | ~0.88   | ~0.78     | ~0.70  |

---

## 🔧 Technologies Used

- Python, Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook

-

---

____________
