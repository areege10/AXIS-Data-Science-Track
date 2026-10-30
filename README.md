# 📊 Telco Customer Intelligence

### An End-to-End Data Science & Machine Learning Project

An interactive customer intelligence dashboard built using Python, Machine Learning, and Streamlit to analyze customer behavior, predict churn, estimate customer revenue, and identify customer segments.

The project transforms raw telecommunications customer data into actionable insights through data analysis, predictive modeling, and interactive visualization.

---

## 🚀 Project Overview

Customer retention and understanding customer behavior are important challenges in the telecommunications industry.

This project aims to explore customer data and develop machine learning models to support business decision-making through four main components:

- **Exploratory Data Analysis (EDA):** Understanding customer characteristics, distributions, and behavioral patterns.
- **Revenue Prediction:** Building a regression model to estimate customer revenue based on the target used during model training.
- **Churn Prediction:** Predicting whether a customer is likely to leave or stay.
- **Customer Segmentation:** Applying clustering algorithms to identify groups of customers with similar characteristics.

An interactive Streamlit dashboard integrates the trained models into a single application.

---

## 🎯 Project Objectives

- Explore and understand telecommunications customer data.
- Perform data cleaning and preprocessing.
- Identify patterns associated with customer churn.
- Develop machine learning models for regression and classification.
- Apply unsupervised learning techniques for customer segmentation.
- Deploy trained models in an interactive dashboard using Streamlit.

---

## 📂 Project Structure

```text
Telco-Customer-Intelligence/
│
├── 01_Data_Preprocessing_EDA.ipynb
├── 02_Regression_CLTV.ipynb
├── 03_Classification_Churn.ipynb
├── 04_Customer_Segmentation.ipynb
│
├── app_Updated.py
│
├── churn_model.pkl
├── cltv_model.pkl
├── kmeans_model.pkl
├── dbscan_model.pkl
├── segment_imputer.pkl
├── segment_scaler.pkl
│
├── telco_customer_segments.csv
│
├── requirements.txt
└── README.md
```

---

## 📓 Project Workflow

### 1. Data Preprocessing & Exploratory Data Analysis

- Examining dataset structure and data types.
- Handling missing values.
- Cleaning and preparing customer records.
- Exploring numerical and categorical variables.
- Investigating customer behavior and churn distribution.
- Visualizing important patterns and relationships.

### 2. Revenue Prediction (Regression)

Developed a regression model to estimate customer revenue using customer-related features.

Main steps:
- Feature selection.
- Data preprocessing.
- Model training and evaluation.
- Saving the trained model for dashboard integration.

**Model output:** Estimated customer revenue.

*Note: The prediction represents the regression target used during model training and should not automatically be interpreted as future customer lifetime value.*

### 3. Customer Churn Prediction (Classification)

Developed a classification model to predict customer churn.

Main steps:
- Selecting relevant customer features.
- Handling numerical and categorical variables.
- Applying preprocessing pipelines.
- Training and evaluating classification models.
- Saving the selected model.

**Model output:**
- Churn: Customer is predicted to leave.
- Stay: Customer is predicted to remain.

The dashboard also displays churn probability when supported by the selected model.

### 4. Customer Segmentation (Unsupervised Learning)

Applied two clustering algorithms:

**K-Means Clustering**
- Identifies customer groups based on similarities in their characteristics.
- Used to assign new customers to existing segments in the dashboard.

**DBSCAN**
- Explores dense customer groups.
- Helps identify noise and potential outlier observations.

Standard DBSCAN does not directly support assigning previously unseen observations using `predict()`. Therefore, K-Means is used for new-customer segment assignment in the dashboard.

---

## 💻 Interactive Streamlit Dashboard

The project includes an interactive dashboard that integrates the trained machine learning models.

**Dashboard Features:**

- Customer information input.
- Churn prediction and churn probability.
- Estimated customer revenue.
- K-Means customer segment assignment.
- DBSCAN methodology explanation.

---

## 🛠️ Technologies & Libraries

| Category | Tools |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Model Serialization | Joblib |
| Dashboard Development | Streamlit |
| Development Environment | Google Colab, Jupyter Notebook |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/areege10/Telco-Customer-Intelligence.git
```

```bash
cd Telco-Customer-Intelligence
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit Application

```bash
streamlit run app_Updated.py
```

The application will open in your browser at the local Streamlit address.

**Important:** Make sure all required trained model files and supporting files are available in the application directory before running the dashboard.

---

## 📊 Dataset

The project uses a telecommunications customer churn dataset containing customer demographic information, subscribed services, account details, charges, and churn-related information.

Dataset dimensions: 7,043 customers and 33 columns in the original dataset.

The dataset was used for preprocessing, exploratory analysis, model development, and customer segmentation.

---

## 📈 Key Learning Outcomes

Through this project, I gained practical experience in:

- End-to-end data science workflow.
- Data preprocessing and exploratory analysis.
- Feature engineering and feature selection.
- Regression and classification modeling.
- Unsupervised machine learning.
- Model evaluation and serialization.
- Integrating machine learning pipelines into a Streamlit application.

---

## 👩‍💻 Author

**Areege Kassab**

Researcher in Environmental Biotechnology

GitHub: [@areege10](https://github.com/areege10)

---

## ⭐ Acknowledgment

This project was developed as part of my continuous learning journey in Data Science and Machine Learning.

Feedback and suggestions are always welcome!
