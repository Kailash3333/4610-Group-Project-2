# 4610-Group-Project-2

Team Members: 

Evelyn Merchant: add user and fork link 

Kailash Konisetty: https://github.com/Kailash3333/4610-Group-Project-2



## Dataset Description


We used the COVID-19 Epidemiological Data dataset from the Snowflake Marketplace, provided by Star Schema / Snowflake Public Data . This dataset includes COVID-19 data from trusted sources like the New York Times, Johns Hopkins University, and The COVID Tracking Project. It contains daily data about cases, deaths, and hospital usage across different locations.

Tables Used (Mainly 3)

1. NYT_US_COVID19
* What it is: Daily COVID-19 case data for U.S. states
* Row count: About 100,000+ rows
* Important columns:
    * DATE (Date): The day of the report
    * STATE (Text): State name
    * CASES (Number): Total cases
    * CASES_SINCE_PREV_DAY (Number): New cases each day
    * DEATHS (Number): Total deaths
* Why we used it: To track how fast COVID cases were increasing over time.


2. CT_US_COVID_TESTS
* What it is: U.S. hospital and testing data
* Row count: About 50,000+ rows
* Important columns:
    * DATE (Date): The day of the report
    * PROVINCE_STATE (Text): State name
    * INICUCURRENTLY (Number): Current ICU patients
    * ONVENTILATORCURRENTLY (Number): Patients on ventilators
* Why we used it: To measure hospital strain, especially ICU and ventilator usage.


3. JHU_COVID_19
* What it is: Global COVID-19 data by country
* Row count: About 1,000,000+ rows
* Important columns:
    * COUNTRY_REGION (Text): Country name
    * PROVINCE_STATE (Text): Region (if any)
    * DATE (Date): The day of the report
    * CASE_TYPE (Text): Type (“Confirmed”, “Deaths”)
    * CASES (Number): Number of cases
* Why we used it: To compare total cases, deaths, and death rates between countries.


How the Tables Connect
* We joined:
    * STATE with PROVINCE_STATE
    * DATE with DATE
This helped us connect:
* COVID case increases → ICU usage → ventilator demand


This dataset is useful because it has a large amount of data and tracks COVID-19 changes daily over time. It includes both case numbers and hospital data like ICU and ventilator usage, which makes it easy to see how rising cases affected hospitals. It also allows us to combine different tables and do more advanced analysis. Using this dataset, we were able to clearly see patterns, like how hospital demand increased after spikes in cases, especially around the January 2021 peak.





## Questions and Justification
## Data Manipulations
## Analysis and Results
## Streamlit App
