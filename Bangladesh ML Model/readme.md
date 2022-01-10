In this project, I wanted to build a model that would forecast some of the economic indicators that play a large role in the functionality of Bangladesh. Aside from the fact that I myself am from there, Bangladesh was a perfect country to analyze in the sense that it is a developing country whose own industrialization and growth is taking place at an unprecedented rate. In contrast to many countries in the West, economic indicators in Bangladesh would tend to fluctuate a lot more because it's such a young country and it's economy is not yet solidified or large enough to have easy forecasts.

DATA DESCRIPTION

The data is in time-series form with continuous quantitative variables from the years 1980 - 2019, containing values on GDP, GDP per-capita, GDP growth, Inflation Rate, Government Debt, Unemployment Rate, and Total Investment. 

EDA


<img width="639" alt="GDP" src="https://user-images.githubusercontent.com/85206295/148713187-02ff6ed3-3f0a-4cfe-a890-d4328bdb1f79.png">

<img width="639" alt="GDPGrowth" src="https://user-images.githubusercontent.com/85206295/148713196-1d38317c-796f-495f-9c15-2ee2bd68765d.png">

<img width="639" alt="InflationRate" src="https://user-images.githubusercontent.com/85206295/148712785-26d9c770-ff71-4125-8a4d-26cad3323fa7.png">

Model

I chose an Autoregressive Integrated Moving Average (ARIMA) model for this task as it can best handle time-series datasets. Based on the EDA, there seemed to be the greatest amount of variance and uncertainty with the trend of the inflation rate, so I chose to predict that. I trained the data on the years 1980 - 2014 and tested it on a series of 5 years (2015 - 2019). To assess the success of this model, I used an  Root Mean Squared Error (RMSE) metric as inflation rate is quantitative continuous. 

Final Model Results

<img width="436" alt="FinalModelResults" src="https://user-images.githubusercontent.com/85206295/148716246-c252de55-6500-44b8-97af-8b1df3730fdb.png">
