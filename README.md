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

![upload_file_google_colab.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/upload_file_google_colab.jpg)

#### Step2: install the following libraries by typing:
```python
!pip install pystan
!pip install prophet
!pip install hvplot
!pip install holoviews
!pip install -U bokeh
!pip install hvplot
    
```
#### Step3: upload data files

use the following code to upload files into google colab:

from google.colab import files
uploaded = files.upload()

after that you can use pd.read_csv to read data files (if in csv format)

![google_colab_upload_files_method.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/google_colab_upload_files_method.jpg)


## Usage

To use the forecasting_net_prophet jupyter lab notebook in google colab, simply clone the full repository and open the **forecasting_net_prophet.ipynb** file in in google colab. 

The tool will go through the following steps:

### Read the search data into a DataFrame, and slice the data
* Import of data to analyze

### Analyze Google search data 2earch for patterns in google search data and vizualize this data
* Group the hourly search data to plot the average traffic by the day of the week
* Visualize traffic as a heatmap
* Group the search data by the week of the year

![mercado_heat_map.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/mercado_heat_map.jpg)

### Relate the Search Traffic to Stock Price Patterns
* Import and plot the stock price data
* Analyze time series for trends
* Create 3 additional data columns
    * Lagged Search Trends (offset search traffic by 1 hour)
    * Stock Volatility with 4 hour rolling average
    * Hourly Stock Return (Percentage stock price change per hour)
* Analyze if predictable relationships exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns


### Create a Time Series Model with Prophet and produce a time series model that analyzes and forecasts patterns in the hourly search data

* Set up the Google search data for a Prophet forecasting model.

* After estimating the model, plot the forecast. How's the near-term forecast for the popularity of MercadoLibre?

* Plot the individual time series components of the model to answer the following questions:

    * What time of day exhibits the greatest popularity?

    * Which day of the week gets the most search traffic?

    * What's the lowest point for search traffic in the calendar year?

![trends_forecast.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/trends_forecast.jpg)


### Forecast Revenue by Using Time Series Models
* Produce a forecast using Prophet for the expected total sales in the next quarter. Include the best- and worst-case scenarios to help them make better plans.

![salesforecast_using_prophet.jpg](https://github.com/nielsdehaan1977/Fintech_Module11/blob/main/Images/salesforecast_using_prophet.jpg)

## Contributor(s)

This project was created by Niels de Haan (nlsdhn@gmail.com)

---

## License(s)

MIT
