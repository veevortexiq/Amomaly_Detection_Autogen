# Anomaly_Detection_Autogen

## Overview
The  script is designed to process and analyze e-commerce order data from a CSV file. It p uploads data to an Elasticsearch instance, retrieves data from Elasticsearch, performs data visualization, and detects anomalies using the ADTK library. The script also includes functionality to interact with an AI agent for anomaly detection.

## Features
1. Elasticsearch Integration
2. Data Visualization
3. Anomaly Detection
4. AI Agent Interaction
   
## Prerequisites
1. Python 3.x 
2. pandas
3. matplotlib
4. elasticsearch
5. adtk
6. autogen (for AI agent interaction)

## Setup
1. Install Required Packages: pip install pandas matplotlib elasticsearch adtk autogen

2. Elasticsearch Setup:
Ensure that you have a running instance of Elasticsearch on localhost at port 9200.
3. Environment Variables:
Set your OpenAI API key as an environment variable

## Output:
1. The script will generate plots showing daily order counts and highlight anomalies.
2. Data will be uploaded and retrieved from Elasticsearch.
3. An AI-generated report will summarize detected order spikes.

## Notes
1. The script assumes the presence of specific columns in the CSV file, such as order_purchase_timestamp, row_number, order_id, and others.
2. Modify the Elasticsearch connection settings if your setup differs from the default configuration (localhost, port 9200).
3. The anomaly detection thresholds can be adjusted in the script (high=350, low=10) based on your dataset characteristics.
