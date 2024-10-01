# Amomaly_Detection_Autogen

## Prerequisites
#### Before running the script, ensure you have the following Python packages installed:
1. adtk
2. autogen
3. pandas
4. matplotlib

## Data Source
The script uses Brazilian e-commerce sales data available on Kaggle. You can download the dataset from Kaggle
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## Script Overview
The script performs the following tasks:
### Data Loading and Preprocessing
1. Loads the dataset olist_orders_dataset.csv.
2. Converts order_purchase_timestamp to datetime format.
3. Resamples data to daily frequency and counts orders per day.
### Data Visualization
1. Plots the daily number of orders over time using Matplotlib.
### Anomaly Detection with ADTK
1. Uses ADTK's ThresholdAD detector to identify anomalies in order counts.
2. Plots detected anomalies on the time series data.
### Custom Tool with Autogen
1. Defines a custom function calculator to preprocess data and detect anomalies based on user-specified dates.
2. Utilizes an assistant agent to analyze anomalies and generate reports.
### Agent Setup and Execution
1. Configures ConversableAgent instances for interaction and anomaly detection.
2. Registers and executes the anomaly detection tool.
## Usage
To run the script, execute it in a Python environment where all prerequisites are installed. The script will automatically process the data, detect anomalies, and provide visualizations.
