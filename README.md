# US Energy Demand and Generation Forecasting

Forecasting of power generation and demand plays an essential role in the electric industry, as it provides the basis for making decisions in power system planning and
operation. In this project, I look at electricity generation and demand data from different regions in the US and apply various time series modeling algorithms to predict
the demand and thereby optimize power generation for these regions for different periods ranging from one hour to one year. 

The datasets used in this project are freely available at the US Energy Information Administration website. I am looking at data from July 2015 to March 2022.
I get the electricity demand data produced by different regions in the US from the following website:
https:// www.eia.gov/electricity/gridmonitor/dashboard/electric_overview/US48/US48

The objective is to forecast Demand and Net Generation values from June 2021 to February 2022.

The granularity of the data hourly. I aggregate the data to generate daily electricity demand and net generation and then perform my analysis.

Balancing Authority(BA) derives its demand value by taking the total metered net electricity generation within its electric system and subtracting the total metered net electricity interchange occurring between the BA and its neighboring BAs. Interchange is nothing but the electricity supplied to the neighboring BA area.

In the dataset that I am working with, I have different Balancing Authorities who report electricity data from specific regions.

The dataset contains electricity demand and net generation values from 13 different regions of the United States.
