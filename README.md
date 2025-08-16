# Capstone-3-Bank-Marketing-Campaign-for-Term-Deposits
# Bank Marketing Prediction

📌 **Project Overview**  
This project focuses on predicting whether a customer will subscribe to a term deposit based on the Bank Marketing dataset using machine learning.  
By leveraging customer and campaign attributes, the model helps financial institutions design cost-efficient marketing strategies and minimize wasted campaign spending.  

---

🗂 **Dataset Information**  
The dataset contains customer and campaign-related features, including:

- **Age**: Customer’s age  
- **Job**: Type of job  
- **Marital**: Marital status  
- **Housing**: Whether the customer has a housing loan  
- **Loan**: Whether the customer has a personal loan  
- **Contact**: Type of communication used (cellular, telephone, unknown)  
- **Month**: Last contact month of the year  
- **Campaign**: Number of contacts performed during this campaign  
- **Pdays**: Number of days since last contact from a previous campaign  
- **Poutcome**: Outcome of the previous marketing campaign  
- **Balance**: Average yearly balance in euros  
- **Deposit**: Target variable (yes = customer subscribed, no = not subscribed)  

---

🎯 **Objectives**
- Perform exploratory data analysis (EDA) to understand data patterns and customer behavior.  
- Preprocess the dataset (handle missing values, encode categorical variables, scale features).  
- Train and evaluate machine learning models to predict deposit subscription.  
- Conduct feature importance analysis to identify the most influential factors.  
- Perform business cost analysis to compare baseline strategies (**Treat All** / **Treat None**) with machine learning strategies.  

---

🛠 **Technologies Used**
- **Python**  
- **Pandas, NumPy** → Data manipulation  
- **Matplotlib, Seaborn** → Data visualization  
- **Scikit-Learn** → Machine learning (Logistic Regression, GridSearchCV)  
- **Jupyter Notebook / Google Colab** → Development environment  

---

🚀 **Project Workflow**

### 1. Data Preprocessing
- Handling missing values and duplicates  
- Encoding categorical variables (OneHotEncoding, LabelEncoding)  
- Scaling numerical features  

### 2. Exploratory Data Analysis (EDA)
- Visualizing distributions of numerical and categorical features  
- Detecting correlations between attributes  
- Understanding customer behavior patterns  

### 3. Baseline Analysis
- **Treat All** → contact all customers  
- **Treat None** → contact no customers  
- Calculate campaign cost vs lost opportunity cost  

### 4. Model Training & Evaluation
- Train Logistic Regression with GridSearchCV for hyperparameter tuning  
- Evaluate using cross-validation and test set metrics (accuracy, recall, precision, F1-score)  
- Focus on **recall**, as missing potential customers (False Negative) is more costly  

### 5. Feature Importance & Interpretation
- Identify key drivers (e.g., housing loan, contact method, previous campaign outcome)  

### 6. Business Cost Evaluation
- Compare ML-driven strategy with Treat All and Treat None  
- Calculate total cost saving and business impact  

---

📊 **Results**

- **Best Model**: Logistic Regression (C=0.01, L2 penalty, solver=saga, max_iter=500)  
- **Best CV Score**: ~0.65  
- **Feature Importance (Top)**: housing, contact, poutcome, loan  

**Cost Comparison**:
- Treat None → **USD 111,150**  
- Treat All → **USD 15,510**  
- Machine Learning → **USD 15,430** (with FN=0)  

✅ Machine Learning strategy achieves the **lowest total cost** and eliminates lost opportunities.  


---

Persyaratan
Python 3.9+
pandas, numpy, matplotlib, seaborn
scikit-learn
category_encoders

---

👩‍💻 **Author**  
Fransiska Sri Mayawi  
Capstone Project 3 — Machine Learning Supervised Classification  


