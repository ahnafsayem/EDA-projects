# Customer Churn EDA

## Overview
This repository contains an Exploratory Data Analysis (EDA) project focused on understanding customer churn in a telecom company. The goal is to analyze factors contributing to customer churn and visualize the data to gain insights.

## Key Findings
From the analysis, we can predict whether a customer is likely to leave (Churn = 1) based on two factors:
- If the customer has made more than 3 calls to customer service.
- If they are subscribed to an International Plan.

If both conditions are met, we predict that the customer is likely to churn (Churn = 1). If not, we predict that the customer will stay (Churn = 0). Using this simple rule, the expected accuracy of the prediction is **85.75%**, indicating that this method would be correct most of the time, with only a small number of cases (373 + 7 = 380) being incorrect. This percentage serves as a good starting point for comparison when building more advanced machine learning models later.

## Contents
- **Data**: The dataset used for the analysis.
- **Notebooks**: Jupyter notebooks with the EDA code and visualizations.
- **Visualizations**: Graphs and charts to illustrate the findings.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook
