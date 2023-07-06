# It's Always Sunny in San Diego: Forecasting Power Consumption with Weather Patterns

This project was completed as part of the final team project for the time series forecasting class in the University of San Diego's Master of Applied Data Science Program.

### Installation
To use this project, first clone the repo on your device using the command below:
```
git init
git clone https://github.com/hunterblum/Energy-Forecasting.git
```

### Objective:

The objective of our project was to forecast hourly energy consumption in San Diego utilizing the previous hour's weather. By accomplishing this goal, we could use our model to have more precise control over the city's many natural gas generators. This would eliminate any wasted power from over-generation and prevent blackouts from under-generation.

### Partners:
* Hunter Blum
* Saba Alemayehu
* Mackenzie Carter

### Methods Used:
* Time Series Forecasting
* Data Visualization

### Technologies Used:
* R

### Description

We began the project by collecting the data from the sources below, with energy data coming from CAISO and weather data coming from the NOAA. We the performed exploratory data analysis, mainly to confirm our belief that energy patterns would follow yearly seasonality (much like the weather!) We also searched for correlations between energy use and our numeric features, finding that the variable, Hourly Wet Bulb Temperature, was highly correlated to our target (energy usage). We then cleaned the data by filling in any missing values using the last observation carried forward. Next, we trained many models ranging from a simple naive forecast and moving average to more complex models like the ARIMA and neural network. In the end, we found that the 2-Hour moving average model was the only model that performed better than our baseline, naive model. Our moving average model had an RMSE of 74 MWh, over two times as accurate as our naive baseline. While this project was a success, we would like to extend its capabilities by getting more precise energy data. We only had access to hourly energy data, however, ideally, we would like to get this down to minute data to have the most impact. 



### Data Sources
Historical hourly load data from EMS (2019-September 2022) : 

http://www.caiso.com/planning/Pages/ReliabilityRequirements/Default.aspx

Historical Hourly San Diego Weather Data (Airport Station from 1/1/2013 to 11/4/2022): 

https://www.ncei.noaa.gov/cdo-web/datatools/lcd

