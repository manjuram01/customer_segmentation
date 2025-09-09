# 📊 Market Segmentation in SBI Life Insurance

## 📝 Overview

This project focuses on **customer segmentation for SBI Life Insurance** using credit card usage behavior. The objective is to group customers into meaningful segments so that the company can provide targeted recommendations such as **savings plans, loans, and wealth management solutions**.

By applying clustering techniques, the project identifies distinct customer groups based on their credit card activity and financial behaviors.

## 📂 Dataset

* **Source**: [Credit Card Dataset (Kaggle)](https://www.kaggle.com/arjunbhasin2013/ccdata)
* **Size**: \~9,000 customers
* **Features**: 18 behavioral variables, including balance, purchases, payments, credit limit, cash advance usage, and tenure.

### Attribute Information (Key Features)

* **BALANCE** – Balance amount left in account
* **PURCHASES** – Total purchases made
* **ONEOFFPURCHASES** – Maximum purchase made in one-go
* **INSTALLMENTSPURCHASES** – Purchases made in installments
* **CASHADVANCE** – Cash taken in advance
* **CREDITLIMIT** – Credit card limit for user
* **PAYMENTS** – Payment amount by user
* **TENURE** – Years of service with the bank
  *(and more – see dataset link for full details)*

## 🔍 Methodology

1. **Data Cleaning** – Handling missing values, removing duplicates, dropping unnecessary columns.
2. **Outlier Detection** – Identified and treated outliers in balance, credit limit, and payments.
3. **Scaling** – Standardized features for fair clustering.
4. **Dimensionality Reduction (PCA)** – Reduced features to 2D for visualization.
5. **Clustering** – Applied **K-Means Clustering**, tested different K values (Elbow Method suggested 4 clusters).
6. **Cluster Analysis** – Interpreted each cluster for business meaning.

## 📊 Key Insights (Customer Segments)

* **Cluster 1 – Transactors**: Low balances, low cash advance, make regular payments (careful spenders).
* **Cluster 2 – Revolvers**: Treat credit card like a loan, high balances, high cash advance, very low full payments (most lucrative for the bank).
* **Cluster 3 – VIP / Prime Customers**: High credit limit, highest full payment percentage, potential for cross-selling premium products.
* **Cluster 4 – Low Tenure Customers**: Newer customers with low balances, opportunity to build loyalty.

## 🛠 Tools & Technologies

* **Python** (Pandas, NumPy, Matplotlib, Seaborn)
* **Scikit-learn** (KMeans, PCA, StandardScaler, Clustering models)
* **Joblib** (model saving)

## 📌 Future Improvements

* The segmentation can be expanded using **hierarchical clustering** and **Gaussian Mixture Models** for comparison.
* Customer demographic and policy data can be integrated for **richer segmentation**.
* The model can be deployed as a **recommendation engine** for insurance advisors.
* Visualization dashboards (Power BI / Tableau) can be added for business presentation.

## 🚀 How to Run

1. Download the dataset from Kaggle and place it in the project directory.
2. Run the Jupyter Notebook / Python script.
3. Trained model (`kmeans_model.pkl`) and segmented dataset (`Clustered_Customer_Data.csv`) will be saved.

## 👤 Author

**Manju Ram Bojja**

* 📧 [manjurambojja@gmail.com](Gmail)
* 🌐 [https://www.linkedin.com/in/manju-ram-b-031976239/](LinkdeIn)
