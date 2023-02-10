# Fintech_Module11

![Prophet_Forecasting.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/Prophet_Forecasting.jpg)

## Forecasting with Prophet, this jupyternotebook can help you to find unusual patterns in google search traffic, search for seasonality, relate search traffic to stock price patterns, create time series Model with Prophet Library and lastely forecast revenue by using the Prophet time series model. 

## forecasting_net_prophet.ipynb
---

### This Jupyter notebook can be used as a template for analyzing search traffic account for seasonality and explore if there is any relationship between search traffic and the stockprice of the company. Lastely the notebook forecast revenues by using Prophet time series model. 

The tool can help with analyzing google search trends the relationship between search trends and the stockprice and forecast revenues using Prophet time series model.  
* notebook goes through the following steps: 
1. Find patterns in google search data for a company
2. Search for seasonal patterns in the data
3. Relate google search traffic patterns to the companies stock price patterns
4. Create a time series model with Prophet 
5. Forecast Revenue by Using Time Series Model

---
## Table of Content

- [Tech](#technologies)
- [Installation Guide](#installation-guide)
- [Usage](#usage)
- [Contributor(s)](#contributor(s))
- [License(s)](#license(s))

---
## Tech

This project leverages Jupyter notebook using Google Colab with the following packages:

* [google_colab](https://colab.research.google.com/) - Colab allows anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. 

* [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html) - Pandas is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.

* [hvplot](https://hvplot.holoviz.org/user_guide/Plotting.html) - hvplot is generate plots from Pandas DataFrames and many other data structures of the PyData ecosystem.

* [holoviews](https://holoviews.org/) - HoloViews is an open-source Python library designed to make data analysis and visualization seamless and simple.

* [Prophet](https://facebook.github.io/prophet/) - Prophet is a forecasting procedure implemented in R and Python. It is fast and provides completely automated forecasts that can be tuned by hand by data scientists and analysts.

* [datetime](https://docs.python.org/3/library/datetime.html) - The datetime module supplies classes for manipulating dates and times.

---

## Installation Guide

### Before running the application first configure a [google colab](https://colab.research.google.com/) for the project. 

#### Step1: Import the downloaded jupyter notebook into google colab. 
```python
    conda activate dev
```
#### Step2: install the following libraries (if not installed yet) by typing:
```python
    pip install pandas
    pip install -U scikit-learn
    conda install -c pyviz hvplot

    
```
#### Step3: Start Jupyter Lab
Jupyter Lab can be started by:
1. Activate your developer environment in Terminal or Git Bash (already done in step 1)
2. Type "jupyter lab --ContentsManager.allow_hidden=True" press enter (This will open Jupyter Lab in a mode where you can also see hidden files)

![JupyterLab](https://github.com/nielsdehaan1977/Fintech_Module10/blob/main/Images/JupyterLab.PNG)


## Usage

To use the crypo_investments jupyter lab notebook, simply clone the full repository and open the **crypto_investments.ipynb** file in Jupyter Lab. 

The tool will go through the following steps:

### Import the Data
* Import of data to analyze

### Prepare the Data
* Prepare data for analysis

### Find the Best Value for k Using the Original Data
* Find the best value for the amount of clusters to use in analysis of original data via elbow method

![elbow_method_graph](https://github.com/nielsdehaan1977/Fintech_Module10/blob/main/Images/elbow.jpg)

### Cluster Cryptocurrencies with K-means Using the Original Data
* Cluster data using KMeans method using original data

![KMeans_org](https://github.com/nielsdehaan1977/Fintech_Module10/blob/main/Images/scatter_org.jpg)

### Optimize Clusters with Principal Component Analysis

* Performs a principal component analysis (PCA) and reduces the features to three principal components

### Find the Best Value for l Using the PCA Data
* Find the best value for the amount of clusters to use in PCA data analysis via elbow method

### Cluster the Cryptocurrencies with K-means Using the PCA Data
* Cluster data using KMeans method using PCA data

### Visualize and Compare the Results
* Visualize elbows and clusters for both original and pca data and compare results

![elbow_compare](https://github.com/nielsdehaan1977/Fintech_Module10/blob/main/Images/elbow_compare.jpg)
![cluster_compare](https://github.com/nielsdehaan1977/Fintech_Module10/blob/main/Images/cluster_compare.jpg)


## Contributor(s)

This project was created by Niels de Haan (nlsdhn@gmail.com)

---

## License(s)

MIT
