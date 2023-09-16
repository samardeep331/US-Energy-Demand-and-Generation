# US Energy Demand and Generation Forecasting

Forecasting of power generation and demand plays an essential role in the electric industry, as it provides the basis for making decisions in power system planning and
operation. In this project, I look at electricity generation and demand data from different regions in the US and apply various time series modeling algorithms to predict
the demand and thereby optimize power generation for these regions for different periods ranging from one hour to one year. 

# Dataset
The datasets used in this project are freely available at the US Energy Information Administration website. I am looking at data from July 2015 to March 2022.
I get the electricity demand data produced by different regions in the US from the following website:
https:// www.eia.gov/electricity/gridmonitor/dashboard/electric_overview/US48/US48
The granularity of the data is hourly. I aggregate the data to generate daily electricity demand and net generation and then perform my analysis. A Balancing Authority(BA) derives its demand value by taking the total metered net electricity generation within its electric system and subtracting the total metered net electricity interchange occurring between the BA and its neighboring BAs. Interchange is nothing but the electricity supplied to the neighboring BA area. In the dataset that I am working with, I have different Balancing Authorities who report electricity data from specific regions. The dataset contains electricity demand and net generation values from 13 different regions of the United States.

# Analysis and Transform
* Time Series Decomposition
* Stationarity test
* Making time series stationary

# Models
* Seasonal Auto-Regressive Integrated Moving Average (SARIMA)
* Prophet

# Evaluation Metric
* Root Mean Squared Error

# Forecasting Results

* Below are the results for the SARIMA model with walk-forward cross-validation
  
 | Region | Demand (RMSE)  | Net Generation (RMSE)  |
| ----- | --- | --- |
| CAL | 46409   | 51347 |  
| CAR | 44610   | 43303 |   
| CENT | 42651   | 44369 | 
| FLA | 48131   | 54091  |    
| MIDA | 166335   | 163746 |  
| MIDW | 82464  | 88585 |  
| NE | 22585   | 22883  |  
| NW | 67907   | 74064   |
| NY | 22914   | 23653  | 
| SE | 50519   | 40384   |
| SW | 67936   | 56846 |  
| TEN | 32694   | 28236 |  
| TEX | 60934   | 59601  | 

* Below are the results for the Prophet model

| Region | Demand (RMSE)  | Net Generation (RMSE)  |
| --- | --- | --- |
| CAL | 52428   | 76937   |
| CAR | 64539   | 56887   |
| CENT | 81117   | 87537   |
| FLA | 149858   | 626415   |
| MIDA | 185093   | 180602   |
| MIDW | 132144  | 139609   |
| NE | 32857   | 34998   |
| NW | 267250   | 249835   |
| NY | 34271   | 37508   |
| SE | 256997   | 71959   |
| SW | 316719   | 273186   |
| TEN | 44294   | 42611   |
| TEX | 108989   | 107149   |

