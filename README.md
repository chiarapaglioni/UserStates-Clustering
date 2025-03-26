# HealthTech AI Hub Hackathon

Team 2 - Challenge 2

### Overview
This project uses unsupervised and supervised machine learning to **cluster athletes' performance states**: 
- overloaded
- underloaded
- balanced

using **self-reported emotional states**, **text reflections**, and **wearable sensor data**. It also includes strategies to **impute missing emotion data** and enhance predictions using partial data.

![pipeline](/plots/user-pipeline.png)

### Project Structure
Below is an overview of the project structure. 

```sh
.
 |-data
 |-plots
 |-EDA.ipynb
 |-Athletes-Clustering.ipynb
 |-Graph_temporal_network.ipynb
 |-Athletes-Prediction.ipynb
 |-Wearable-Data.ipynb
 |-requirements.txt
```

where: 
- **data**: 
    - folder containing data in CSV format
- **plots**: 
    - folder containing plots and figures
- **EDA.ipynb**: 
    - Performs EDA and Data Analysis of datasets
- **Athletes-Clustering.ipynb**: 
    - Data Preprocessing of __raw_data.csv__ 
    - uses an NLP based approach to predict missing emotion values
    - performs clustering of complete data with KMeans and visualise it with PCA
- **Graph_temporal_network.ipynb**: 
    - Data Preprocessing of the __raw_data.csv__  
    - uses an Graph based approach to predict missing emotion values
    - performs clustering of complete data with KMeans and visualise it with PCA
- **Athletes-Prediction.ipynb**: 
    - predicts the clusters new users are going to be in based on the clusers predicted from the NLP and Graph based approach
- **Wearable-Data.ipynb**: 
    - performs EDA and Data Preprocessing of __wearable_users_raw_data.csv__ 

## Installation and setup instructions
This project requires **Python 3.9**. The dependencies are listed in the _requirements.txt_ file and can be installed via pip as follows:

```sh
pip install -r requirements.txt
```