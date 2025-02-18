# Kedro


## Introduction 
Kedro is an open-source Python framework for creating reproducible, maintainable, and modular data science code.
Developed by QuantumBlack, a McKinsey company, Kedro aims to standardize the process of building data pipelines.

# Features
Pipeline Management: Organize your data engineering code into pipelines, each consisting of nodes that perform specific tasks.
Data Catalog: A YAML-based configuration file that specifies how and where datasets are stored, making it easy to manage data inputs and outputs.
Modular Pipelines: Support for creating reusable and shareable pipeline components.
Experiment Tracking: Integration with Kedro-Viz for visualizing and tracking experiments.
# Project Structure 
 
Open Screenshot 2024-11-11 at 5.39.38 PM-20241111-120943.png

 
# Use Case 1 : Dataset registration
The following information about a dataset must be registered before Kedro can load it:
File location (path)
Parameters for the given dataset
Type of data
Versioning
Install Kedro (v 0.19.0)
Open Screenshot 2024-11-11 at 3.59.43 PM-20241111-102948.png

# Requirements 
 
Open Screenshot 2024-11-11 at 4.01.25 PM-20241111-103130.png

Loading the Dataset named companies.csv
 
Open Screenshot 2024-11-11 at 4.02.46 PM-20241111-103251.png

Loading the Dataset named shuttles.xlsx
 
Open Screenshot 2024-11-11 at 4.03.48 PM-20241111-103354.png

We are able to load the data which is registered with Kedro. 
 
Use Case 2: Running Data science pipeline
Run node 1 : preprocess_companies_node
Open Screenshot 2024-11-11 at 4.05.52 PM-20241111-103558.png

Check the status 
Open Screenshot 2024-11-11 at 4.07.00 PM-20241111-103705.png

Run node 2 : preprocess_shuttles_node and status check
Open Screenshot 2024-11-11 at 4.07.00 PM-20241111-103705.png

Visualize the pipeline 
Here the third dataset named as Review is included so that master data can be prepared.
Open Screenshot 2024-11-11 at 4.09.03 PM-20241111-103908.png

Pipeline will look something like this 
Open Screenshot 2024-11-11 at 3.49.54 PM-20241111-102001.png

Several pointers before considering - 
Not fully functional in terms of version ( Tried latest version of Kedro with latest python but it shows incompatibility)
 
Open Screenshot 2024-11-11 at 4.11.38 PM-20241111-104144.png

Teams should have strong devops knowledge in terms of manifest/yaml to understand the workflow. 
Kedro still need to be tested for scalability and  teams collaboration.
 

Add label

