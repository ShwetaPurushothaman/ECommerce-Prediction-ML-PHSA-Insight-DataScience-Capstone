# E-Commerce Capstone Project

This repository contains the code and materials related to the E-commerce Capstone project by **Shweta Purushothaman**. The project focuses on analyzing a dataset from an international e-commerce company to gain insights into customer behavior, product shipments, and applying various machine learning models to improve shipment tracking.

## Table of Contents
<!--ts-->
  * [Project Overview](#project-overview)
  * [Dataset Information](#dataset-information)
  * [Project Objectives](#project-objectives)
  * [Tools and Technologies Used](#tools-and-technologies-used)
  * [Installation Guide](#installation-guide)
  * [Project Structure](#project-structure)
  * [Machine Learning Models](#machine-learning-models)
  * [Results](#results)
  * [How to Run the Project](#how-to-run-the-project)
  * [License](#license)
<!--te-->

## Project Overview
The E-commerce company provides electronic products and is interested in discovering key insights using advanced machine learning techniques. The project explores shipment tracking and customer satisfaction by analyzing features such as customer ratings, product importance, shipment modes, and more. Machine learning models are applied to classify shipments delivered on time or not.

## Dataset Information
The dataset used for this project contains **10,999 observations** and **12 variables**, including:
- `ID`: Customer ID.
- `Warehouse block`: Warehouse is divided into sections (A, B, C, D, E).
- `Mode of shipment`: Shipment modes (Ship, Flight, Road).
- `Customer care calls`: Number of customer calls for shipment inquiries.
- `Customer rating`: Rating from 1 (Worst) to 5 (Best).
- `Cost of product`: Price in US dollars.
- `Prior purchases`: Number of prior purchases made by the customer.
- `Product importance`: Categorized as low, medium, or high.
- `Gender`: Male or Female.
- `Discount offered`: Discount provided on the product.
- `Weight in grams`: Weight of the product.
- `Reached on time`: Target variable (1 = Not on time, 0 = On time).

## Project Objectives
- Predict whether shipments are delivered on time or not.
- Analyze customer ratings and the impact of product importance on delivery.
- Apply machine learning models and evaluate their performance.
- Provide visual insights and recommendations.

## Tools and Technologies Used
- **Python**: The primary language used for data analysis and machine learning.
- **Jupyter Notebook**: For writing and executing the code.
- **Pandas, NumPy**: For data manipulation and analysis.
- **Matplotlib, Seaborn**: For data visualization.
- **Scikit-learn**: For implementing machine learning models.
- **Tableau**: For visualizing using dashboard.

## Installation Guide

To run this project locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/ecommerce-capstone.git
    cd ecommerce-capstone
    ```

2. **Set up a virtual environment** (recommended):
    ```bash
    python -m venv env
    source env/bin/activate   # On Windows: env\Scripts\activate
    ```

3. **Install dependencies**:
    Install the required Python libraries using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

4. **Open Jupyter Notebook**:
    Start the Jupyter notebook server:
    ```bash
    jupyter notebook
    ```
    Open the `ShwetaPurushothaman_E-commerce_Capstone.ipynb` file in the Jupyter notebook.

## Project Structure

The repository is structured as follows:
```bash
/project-repo
    ├── Dataset/
    │    └── Description.md 
    │    └── E_Commerce.csv
    │ 
    ├── Presentation/
    │    └── Description.md 
    │    └── ShwetaPurushothaman_E-commerce_Capstone.pptx
    │ 
    ├── Python Notebook/
    │    └── Description.md 
    │    └── ShwetaPurushothaman_E-commerce_Capstone.ipynb
    │ 
    ├── Tableau/
    │    └── Description.md 
    │    └── ShwetaPurushothaman_E-commerce_Capstone.twb
    │ 
    └── README.md
```

* [Dataset](./Dataset/E_Commerce.csv/)                          # Directory containing the dataset
* [Presentation](./Presentation/)                          # Directory for storing PPT
* [Python Notebook](./Python%20Notebook/ShwetaPurushothaman_E-commerce_Capstone.ipynb/)  # Main project notebook
* [Tableau](./Tableau/)               # Directory for Tableau file 
* README.md                        # This README file

## Machine Learning Models

Several machine learning models are applied to predict the target variable (`Reached on time`):

- **Logistic Regression**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

Each model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.

## Results

- The project analyzes the relationship between different variables, such as customer care calls, customer ratings, and shipment delivery times.
- Machine learning models are compared based on their performance to determine the best fit for the dataset.

## How to Run the Project

1. Clone this repository to your local machine.
2. Set up your environment and install the necessary dependencies.
3. Open the Jupyter notebook and run the cells to execute the code step by step.
4. Review the output graphs and model evaluations to understand the insights generated by the dataset.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
