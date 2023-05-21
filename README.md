# energy-forecasting-time-series-model



# Energy Consumption Analysis and Forecasting



## Project Overview

This project is an in-depth analysis and forecasting of energy consumption data using various machine learning and data analysis techniques. The goal of this project is to provide insights into patterns of energy use and to predict future energy consumption, which could be useful in resource allocation, energy conservation strategies, and infrastructure planning.

## Data Source

The dataset employed in this context comprises of energy consumption readings in kilowatt-hour (kWh) collected from a sample of London households during the period between November 2011 and February 2014 from [SmartMeter Energy Consumption Data in London Households](https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households). This time-series data, inherently structured around precise timestamps, possesses the potential to reveal invaluable insights into the patterns and trends of energy usage over time.

The data used in this project is sourced as part of the data, i.e. the "LCL-June2015v2_1.csv" file. This dataset contains half-hourly energy consumption data, which we analyze and model to gain insights and make predictions.

## Methodology

### Data Preprocessing

The data is loaded from the CSV file and cleaned to handle missing or misformatted data. The `DateTime` column is parsed into a datetime format and set as the index of the dataframe, facilitating time series analysis.

### Exploratory Data Analysis

The data is then analyzed using various data visualization techniques such as line plots, scatter plots, histograms, boxplots, and heatmaps. This process involves exploring the distribution of energy consumption and its relationships with different variables such as date, time of day, month, and year.

### Trend Analysis by Resampling

We also performed trend analysis to understand the patterns of energy usage over different periods (daily, weekly, yearly). Rolling means and differences were also plotted to understand patterns in the data.

### Hierarchical Clustering

A dendrogram was generated to perform hierarchical clustering on the energy consumption data. This approach allowed us to identify similar hours of the day in terms of energy consumption.

### Forecasting with Prophet

For forecasting energy consumption, we used Prophet, a procedure for forecasting time series data. Prophet's predictive power comes from its ability to handle trends, seasonality, and holidays, which are common in many time series datasets.

### Machine Learning: LSTM Model

To further improve the accuracy of our predictions, we also trained a Long Short-Term Memory (LSTM) network on the energy consumption data. This type of recurrent neural network is capable of learning patterns over time, making it suitable for time series forecasting. The LSTM model was tuned using Keras Tuner to optimize its architecture and hyperparameters. The model was then used to make predictions on the training and test datasets.

## Project Impact

This project provides insights into energy consumption patterns and accurately predicts future consumption. These findings can aid in decision-making processes related to energy management, infrastructure development, and sustainability initiatives. Predicting energy usage can also help in devising strategies for efficient energy utilization, leading to cost savings and reduced environmental impact.