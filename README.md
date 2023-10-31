# DataMing Project
### Xiaoya Huang, Xiyu Li, Elsie Ye, Wenpei Zhao, Yu Zhao

## Research Questions
 1. For the selected routes between LAS and LAX, what will be the reason that caused different types of delay?

 2. Could we create models to predict the delay?

## Data Source
https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGK

https://www.visualcrossing.com/weather-data


## Data Sets
For flight data, we filter the original monthly data to the flights between LAX and LAS airport and select the first 70 columns. Then we combined all the monthly data together to the following datasets:

`flights1819.csv`: flights data from June 2018 to December 2021

`flight20.csv`: flights data from Jan 2020 to Dec 2020

`flight2021.csv`: flights data from Jan 2021 to Dec 2021

`flights2223.csv`: flights data from January 2022 to May 2023

`DataDictionary.html`: Data dictionary for the dataset

For weather data

`LasVegasWeather.csv`:  Las Vegas weather data from May 2018 to May 2023

`LosAngelesWeather.csv`:  Los Vegas weather data from May 2018 to May 2023

`weatherdatadic.html`: data dictionary for the weather dataset

## Data Processing: 

Step 1: Data Column Removal
In the initial dataset, there were 103 columns. After data preprocessing, we retained only the relevant columns, resulting in an updated dataset named "flight_ALL.csv" with 46 columns.

Step 2: Time Format Standardization
To ensure consistency, the time format for both Arrival and Departure data was standardized. All time entries were converted to the format "12:30" represented as "1230."

Step 3: Handling Missing Data
In the dataset, some entries in the "ArrDelay" variable were missing (NA). To address this, missing values were filled in, ensuring the completeness of the data for further analysis.
