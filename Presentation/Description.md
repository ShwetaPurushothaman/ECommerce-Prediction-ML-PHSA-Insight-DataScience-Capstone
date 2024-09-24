# E-commerce Capstone Project: Presentation Overview

## Overview

This presentation outlines the key aspects of the E-commerce Data Science Capstone project. The project involves analyzing a dataset from an international e-commerce company to derive insights on customer behavior and delivery performance using machine learning models.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Overview](#data-overview)
3. [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
4. [Feature Engineering](#feature-engineering)
5. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
6. [Modeling Approach](#modeling-approach)
7. [Model Performance](#model-performance)
8. [Insights and Findings](#insights-and-findings)
9. [Recommendations](#recommendations)
10. [Challenges and Limitations](#challenges-and-limitations)
11. [Future Work](#future-work)
12. [Conclusion](#conclusion)

## Introduction

The project aims to answer key business questions such as:
- What is the customer rating for each product?
- Was the product delivered on time?
- How does product importance affect customer satisfaction and delivery times?

The data is used to build machine learning models to provide actionable insights for improving customer experience and delivery logistics.

## Data Overview

The dataset contains 10,999 observations with 12 variables, including:
- **ID**: Unique customer identifier
- **Warehouse Block**: Shipping warehouse
- **Mode of Shipment**: Shipping method (Ship, Flight, Road)
- **Customer Care Calls**: Number of customer inquiries
- **Customer Rating**: Rating from 1 to 5
- **Cost of Product**: In USD
- **Product Importance**: Categorized as Low, Medium, High
- **Reached on Time**: Target variable (1 = Not reached on time, 0 = Reached on time)

## Data Cleaning and Preprocessing

- The dataset contained no missing or duplicate records.
- Outliers were detected in `Prior_purchases` and `Discount_offered`, which were handled using box plot techniques.
- Categorical variables were encoded, and unimportant features like `Gender` and `ID` were removed using Recursive Feature Elimination (RFE).

## Feature Engineering

- Numerical encoding was applied to categorical variables.
- Features that did not contribute to model performance, like `Gender` and `ID`, were removed.

## Exploratory Data Analysis (EDA)

Key insights were derived by visualizing:
- The mode of shipment: Ship was the most used method, followed by Flight and Road.
- Product importance: Most shipments were categorized as Low or Medium importance.
- Customer ratings and delivery times: Products that arrived late had lower customer ratings.

## Modeling Approach

The goal was to predict whether a product would be delivered on time (binary classification). Several machine learning models were implemented:
- **Naive Bayes (Bernoulli)**
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Machines (SVM)**
- **Decision Tree**
- **Boosting & Bagging Decision Trees**
- **Random Forest Algorithm**

The dataset was split into training (80%) and testing (20%) sets.

## Model Performance

The Random Forest algorithm performed the best in terms of:
- **Accuracy**
- **ROC-AUC Score**
- **Precision and Recall**

GridSearchCV was used for hyperparameter tuning to optimize model performance.

## Insights and Findings

- **Random Forest** was the best-performing model, providing the most accurate predictions.
- Products with higher importance but low ratings were often delayed.
- An increase in customer care calls correlated with delays in delivery.

## Recommendations

- Improve delivery times by:
  - Optimizing capacity planning.
  - Enhancing demand forecasting.
  - Streamlining the supply chain.
  - Improving inventory management.
  
## Challenges and Limitations

- The dataset exhibited skewness and kurtosis, which affected some models.
- Challenges included selecting the best machine learning models and handling noisy data.

## Future Work

- Implement additional machine learning techniques, such as deep learning models.
- Use advanced hyperparameter tuning methods like GridSearchCV earlier in the model-building process.
- Extend the analysis to include different data splits and other ensemble learning techniques, like stacking.

## Conclusion

The project concludes that the **Random Forest** algorithm, with Decision Tree as the base model, provides the best predictive performance for on-time delivery. This model can be used to optimize delivery processes and improve customer satisfaction.

## Dashboard and Presentation Links

- **Tableau Dashboard**: [View the Dashboard](https://public.tableau.com/app/profile/shweta.purushothaman/viz/ShwetaPurushothaman_E-commerce_Capstone/Dashboard1?publish=yes)
- **Presentation**: [View the Presentation](./Presentation/)
