# ctCeSj7pq6D28iNU

# Predictive Customer Satisfaction Analysis

This repository contains a machine learning pipeline aimed at solving a real-world industry problem: predicting customer dissatisfaction in a logistics and delivery business. The goal is to enable the company to proactively improve services based on actionable insights derived from customer feedback.

## Project Background

**From Data Exploration to Predictive Insights:**

In the fast-paced logistics industry, ensuring customer satisfaction is crucial. I worked with a client to uncover that 45.24% of their customers were dissatisfied, a significant issue that could affect business growth. This analysis was part of my experience with the Apziva AI Residency program, where the original goal was to predict happy customers. However, realizing that almost half of the customer base was unhappy, we shifted our focus to predicting dissatisfied customers, allowing the client to make targeted improvements.

### Problem Context

The client is a global logistics startup that partners with multiple vendors to deliver services. They conducted a customer satisfaction survey covering key aspects of the delivery process:

- **X1:** Timely delivery
- **X2:** Accuracy of order contents
- **X3:** Completeness of order
- **X4:** Value for money
- **X5:** Courier satisfaction
- **X6:** Ease of use of the app

The company’s goal was to predict customer dissatisfaction (class 0) to focus on service improvements and better understand where their processes needed attention. This shift helped the company address customer needs in real-time and prevent further dissatisfaction, contributing to increased loyalty and retention.

## Project Overview

1. **Exploratory Data Analysis** (`exploratory_analysis.ipynb`):
   - Cleaned, preprocessed the dataset, and visualized the relationships between survey responses.
   - Identified key factors leading to dissatisfaction and analyzed trends using univariate and bivariate analysis.

2. **Model Training** (`prediction_model_training.ipynb`):
   - Built a machine learning model using Random Forest to predict customer dissatisfaction.
   - Hyperparameter tuning and feature engineering helped optimize the model to exceed the accuracy threshold while focusing on predicting unhappy customers.

---
# **Conclusion**:
1. Almost **half of the customers** are **unhappy**, which is a **big loss** for the business

    - **Happy customers:** 54.76%
    - **Unhappy customers:** 45.24% 

2. **Majority** of the customers are **happy** with the **Courier Service**
3. Almost **half** of the packages are being **delivered with incorrect items**
4. **Most** customers **(~ 83 %)** have **ordered what they wanted to order**
5. **Almost all** customers think **pricing for products and service** is *good* **(~ 94 %)**
6. **Most** customers are happ**y** with the courier service **(~ 82 %)**
7. **Almost all** are **happy** with the **app** as it **makes ordering easy** for them **(~ 98.4 %)**

# **Recommendations for the Company:**

- **X2 :** *contents of my order was as I expecte*d , **X1 :** my order was delivered on time and **X5:** *I am satisfied with my courier* are the **top 3 features** to focus on for **customer satisfaction** and **avoiding unhappy customers**

- From the **top 3 features** the **most important** one is: **X5: I am satisfied with my courier**

Most people have **rated 3 or lower** which is causing **half of the customers to be unhappy** , so the company needs to immidiately fix this as this is a **major loss** for the company

- Another **2 services** that can be **improved** are:
    
    - **X3:** *I ordered everything I wanted to order* 
    - **X5:** *I am satisfied with my courier*
    
    as there are more customers who rated this feature **below 3 — particularly 1 or 2** — compared to other features, which could be contributing to **half of the customers** feeling dissatisfied.

- Customers are **highly satisfied** with the **remaining 3 services** so keep up the good work here:

    - **X1:** *my order was delivered on time*
    - **X4:** *I paid a good price for my order*
    - **X6:** *the app makes ordering easy for me*


# **what was acheived:**

- Figured out the **most important** features:

    - **X5** and **X2** are the **most important** features

- Figured out that almost **half** of the customers are unhappy based on the percentage of happy vs unhappy customers which is:

    - *Happy customers:* **54.76%**
    - *Unhappy customers:* **45.24%**

- Figured out the **best model** to predict *class 0 unhappy customers* as this should be the main focus of the business since they are **almost half** and the best model is **Xgboost** which has an **f1 score** of **0.73** after performing **state of the art hyperparameter optimizations**


# **Summarize What You Did:**

- **Performed exploratory data analysis** to understand the dataset  
- **Identified key factors** leading to dissatisfaction and analyzed trends using *univariate analysis*  
- **Built and tested the best machine learning model** using techniques such as *RFE*, resulting in the best model — **XGBoost** — with a final **F1 score of 0.73 for class 0** to predict customer dissatisfaction  
- **Hyperparameter tuning and feature engineering** helped optimize the model to exceed the accuracy threshold, with a focus on predicting unhappy customers — improved from **0.67** to **0.73**, which is a **6% increase**  
- **Saved the best performing model** to a file for future use  
- **Provided conclusions and recommendations** for the company based on the **analysis** and **model performance**

---

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/osamaizhar/ctCeSj7pq6D28iNU
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebooks:
   - Start with `exploratory_analysis.ipynb` to clean and explore the data.
   - Proceed to `prediction_model_training.ipynb` to train and optimize the predictive model.

## License
This project is licensed under the MIT License.
