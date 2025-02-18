# Kedro


## Introduction 
Kedro is an open-source Python framework for creating reproducible, maintainable, and modular data science code.
Developed by QuantumBlack, a McKinsey company, Kedro aims to standardize the process of building data pipelines.

## Features
1. Pipeline Management: Organize your data engineering code into pipelines, each consisting of nodes that perform specific tasks.
2. Data Catalog: A YAML-based configuration file that specifies how and where datasets are stored, making it easy to manage data inputs and outputs.
3. Modular Pipelines: Support for creating reusable and shareable pipeline components.
4. Experiment Tracking: Integration with Kedro-Viz for visualizing and tracking experiments.
## Project Structure 
 
![EE7D92F1-0A79-40A9-A403-48FC03A52D11_4_5005_c](https://github.com/user-attachments/assets/9b7e1652-babf-4de8-8fd7-5a8208e3d773)


 
## Use Case 1 : Dataset registration
The following information about a dataset must be registered before Kedro can load it:
1. File location (path)
2. Parameters for the given dataset
3. Type of data
4. Versioning
5. Install Kedro (v 0.19.0)

![D3669863-413A-4EBB-B241-B291D349C4C0](https://github.com/user-attachments/assets/4d19958b-fa73-479b-addd-9d75a0444a55)

Requirements 
 
![9F360DA8-FE99-4109-8262-3CD4A697FD7D_1_105_c](https://github.com/user-attachments/assets/f9df1296-092c-4ad1-8cbe-1ef1049f3754)


Loading the Dataset named companies.csv
 
![B4D6DA55-CF2D-4CE7-B5CB-13D4A73BD50B_4_5005_c](https://github.com/user-attachments/assets/1e71e851-ced3-4721-afb2-594a2de2fcd8)


Loading the Dataset named shuttles.xlsx
 
![CDB6437C-119E-422B-89A3-456AA81D584C_4_5005_c](https://github.com/user-attachments/assets/9ff74d0d-f83d-4d54-b052-d4a5a0c9a703)


We are able to load the data which is registered with Kedro. 
 
## Use Case 2: Running Data science pipeline
Run node 1 : preprocess_companies_node
![371EF122-E3B0-427D-96DF-F9E7BC355E65](https://github.com/user-attachments/assets/7cb24329-06c1-4498-9d97-6f91b05361b7)


Check the status 
![8D7EDF36-A4D7-4FC4-A34B-28A06B42DF70](https://github.com/user-attachments/assets/85892a48-91ae-4d38-94be-b8a3becfdb73)

Run node 2 : preprocess_shuttles_node and status check



Visualize the pipeline 
Here the third dataset named as Review is included so that master data can be prepared.
![CA221E40-0760-41EC-9D44-7BBB1BEEE564](https://github.com/user-attachments/assets/636accf9-835f-4566-93aa-898596950fcd)


Pipeline will look something like this 
![92B23106-9050-4A5D-A1BB-B930D11317E9](https://github.com/user-attachments/assets/56522856-db20-4e3a-b699-9aa5a0f8ed18)



Several pointers before considering - 
Not fully functional in terms of version ( Tried latest version of Kedro with latest python but it shows incompatibility)
 
![Uploading B7054488-3230-425A-82EC-A55336270486_4_5005_c.jpeg…]()


Teams should have strong devops knowledge in terms of manifest/yaml to understand the workflow. 
Kedro still need to be tested for scalability and  teams collaboration.
 

Add label

