# E-commerce Data Science Capstone Project

## Project Overview

This project focuses on analyzing an international e-commerce company's dataset. The objective is to discover key insights using advanced machine learning techniques to understand customer behavior, sales performance, and improve delivery times. The project involves several phases, including data cleaning, preprocessing, feature engineering, exploratory data analysis (EDA), and applying machine learning models to predict delivery outcomes.

## Table of Contents

- [Introduction](#introduction)
- [Data Overview](#data-overview)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling Approach](#modeling-approach)
- [Model Performance](#model-performance)
- [Insights and Findings](#insights-and-findings)
- [Recommendations](#recommendations)
- [Challenges and Limitations](#challenges-and-limitations)
- [Future Work](#future-work)
- [Conclusion](#conclusion)
- [Dashboard and Presentation](#dashboard-and-presentation)

## Introduction

An international e-commerce company, specializing in electronic products, seeks insights from its customer database. The aim is to use machine learning models to address key questions such as:
- **What is the customer rating for each product?**
- **Was the product delivered on time?**
- **Are customer queries being addressed effectively when product importance is high?**

## Data Overview

The dataset used for model building contains 10,999 observations and 12 variables, including:
- **ID**: Customer identifier.
- **Warehouse block**: Warehouse section (A-E).
- **Mode of shipment**: Ship, Flight, or Road.
- **Customer care calls**: Number of customer service calls.
- **Customer rating**: Rating on a scale from 1 (Worst) to 5 (Best).
- **Cost of the product**: Product cost in USD.
- **Prior purchases**: Number of prior purchases by the customer.
- **Product importance**: Low, Medium, or High.
- **Gender**: Customer gender.
- **Discount offered**: Discount on the product.
- **Weight in grams**: Product weight.
- **Reached on time**: Target variable (1 = Not reached on time, 0 = Reached on time).

## Data Cleaning and Preprocessing

- **Data Inspection**: Dataset has 10,999 rows and 12 columns, with no missing or duplicate records.
- **Outlier Detection**: Outliers identified in the `Prior_purchases` and `Discount_offered` columns using Box Plot techniques.
- **Outlier Treatment**: Outliers removed based on upper and lower range limits.

## Feature Engineering

- **Feature Selection**: Recursive Feature Elimination (RFE) identified unimportant features such as `Gender` and `ID` for removal.
- **Feature Extraction**: Categorical data (e.g., `Warehouse_block`, `Mode_of_Shipment`, `Product_importance`) were encoded into numerical format for model building.

## Exploratory Data Analysis (EDA)

Key visualizations and analyses include:
- **Mode of shipment**: Most shipments were made by Ship, followed by Flight and Road.
- **Product importance**: Majority of shipments had products with low or medium importance.
- **Customer ratings**: Higher ratings are correlated with products that arrived on time, and the highest unreached products were rated 3.

## Modeling Approach

For the target variable `Reached on time (0/1)`, we used binary classification models. Several machine learning techniques were implemented, including:
- **Naive Bayes (Bernoulli)**
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machines (SVM)**
- **Decision Tree**
- **Boosted Decision Tree**
- **Bagging Decision Tree**
- **Random Forest Algorithm**

The dataset was split into training (80%) and testing (20%) sets, with model performance measured using metrics like accuracy, ROC-AUC, and F1-score.

## Model Performance

After evaluating multiple models, the **Random Forest Algorithm** provided the best results. The models were compared based on:
- **Accuracy**: Random Forest had the highest accuracy.
- **Precision, Recall, and F1-score**: Random Forest outperformed other models.
- **Cross-validation** and **ROC-AUC** were used to ensure model robustness.

## Insights and Findings

- The best-performing model was **Random Forest**, followed by Decision Tree and Logistic Regression.
- Products with high importance but low ratings tend to have higher delivery delays.
- Customer care calls were higher for shipments that did not arrive on time.

## Recommendations

- **Capacity Planning**: Optimize the number of items that can be processed and delivered on time.
- **Demand Forecasting**: Anticipate future demand to allocate resources effectively.
- **Supply Chain Optimization**: Collaborate with suppliers and logistics partners to improve delivery times.

## Challenges and Limitations

- **Data Skewness**: Some variables exhibited skewness and kurtosis, affecting model performance.
- **Model Selection**: Choosing the right model required extensive tuning and cross-validation.
- **Outliers**: Dealing with outliers in `Prior_purchases` and `Discount_offered` was challenging.

## Future Work

- Implement more machine learning models, including deep learning.
- Use advanced techniques like **stacking ensemble** learning to improve accuracy.
- Explore different data splits (e.g., 70-30, 60-40) and compare results.

## Conclusion

After evaluating multiple models, the **Random Forest Algorithm** emerged as the best-performing model for predicting whether a product will be delivered on time. This model offers accurate, reliable predictions and can help the company optimize its delivery process.

## Dashboard and Presentation

- **Tableau Dashboard**: An interactive Tableau dashboard was created to visualize insights from the data. You can access the dashboard [here](https://public.tableau.com/app/profile/shweta.purushothaman/viz/ShwetaPurushothaman_E-commerce_Capstone/Dashboard1?publish=yes).
- **Project Presentation**: A detailed project presentation is available that explains the methodology, insights, and model performance. [View the presentation](link-to-presentation).

