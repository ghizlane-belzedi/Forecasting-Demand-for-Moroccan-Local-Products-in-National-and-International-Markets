# Forecasting Demand for Moroccan Local Products in National and International Markets: A Data-Driven Approach

This repository contains the code and data for the project titled "Forecasting Demand for Moroccan Local Products in National and International Markets: A Data-Driven Approach" by BELZEDI Ghizlane & DAOUDI Halima.

## Overview

In this project, we explore the demand for Moroccan local products in both national and international markets using a data-driven approach. We analyze various datasets related to export values, growth in export values, and the share of export values by product. The goal is to develop models that can forecast demand for these products over time.

## Data Exploration

We start by exploring the available datasets:

- `exported_value.csv`: Contains export values of Morocco from 2003 to 2022.
- `export_value_growth.csv`: Contains the percentage growth in export value from 2003 to 2022.
- `share_of_country_cluster_exports.csv`: Contains the share of export values in the country's cluster exports from 2003 to 2022.

We visualize the data to understand trends and patterns in export values, growth rates, and market shares for different products.

## Data Cleaning and Preprocessing

After exploring the data, we perform cleaning and preprocessing steps, including handling missing values, normalizing data, and creating temporal sequences for model training. We also divide the data into training and testing sets for model evaluation.

## Model Training

### LSTM Model

We train a Long Short-Term Memory (LSTM) model to forecast demand for Moroccan local products. The model takes into account temporal dependencies in the data and is trained using the preprocessed sequences. We evaluate the model's performance using metrics such as Mean Squared Error (MSE) and visualize predictions against actual values.

### ARIMA Model

Additionally, we utilize the AutoRegressive Integrated Moving Average (ARIMA) model to forecast demand for each product. We fit ARIMA models to individual product data and evaluate their performance using RMSE. The results are compared across different products to assess the overall forecasting accuracy.

## Results

We present the results of both the LSTM and ARIMA models, including evaluation metrics and visualizations of predictions. The models provide insights into the demand dynamics of Moroccan local products and can aid decision-making in marketing and production planning.

## Files and Directory Structure

- `data/`: Contains the raw and processed datasets.
- `models/`: Contains trained LSTM and ARIMA models.
- `notebooks/`: Jupyter notebooks used for data exploration, preprocessing, and model training.
- `README.md`: This file providing an overview of the project.

## Requirements

The project requires Python 3.x with the following libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tensorflow
- statsmodels

You can install the required dependencies using pip:

```bash
pip install -r requirements.txt
