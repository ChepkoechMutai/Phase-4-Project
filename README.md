**Predictive Time Series Modeling for Real Estate Investment using Zillow Research Data**

# 1.Introduction

Real estate refers to land, buildings, and other physical property, including natural resources such as crops, minerals, or water, that can be bought, sold, leased, or rented for various purposes. Real estate is a significant part of the global economy and is used for residential, commercial, industrial, and agricultural purposes. Real estate investments can provide both short-term and long-term returns through rental income, property appreciation, and value-added investments such as renovations and developments.


With a population of over 330 million, The real estate industry in the USA is a significant contributor to the country's economy, accounting for approximately 6% of the Gross Domestic Product (GDP). This industry comprises of various sub-sectors, including residential and commercial real estate, real estate development, property management, and real estate investment trusts (REITs).

Residential real estate is the largest sub-sector, accounting for the majority of real estate transactions in the country. The demand for residential real estate is driven by factors such as population growth, household formations, and employment opportunities. The commercial real estate sector, which includes office buildings, retail spaces, and industrial properties, also plays a significant role in the economy, with businesses relying on these properties to operate and grow.

# 2.Business Understanding
**i.Problem Statement**

Real estate represents a significant portion of most people's wealth, and this is especially true for many homeowners in the United States. A number of factors drive the real estate market including government policies, demographics of the potential buyers,affordability, disparity in housing access, location, cash flows and liquidity as well as the current economic climate. The many variables can make the process tedious for the buyers. Newbie consultants hopes to create a predictive time series model that can help to determine the top five zipcodes in which to invest in.

**ii.Main Objective**

The main objective of this project is to develop a time series model that can predict the future prices of houses for Newbie Investments to invest in.

# 3.Notebook Structure
* Data Cleaning
* External Data Validation
* Exploratoratory Data Analysis
* Data Preprocessing
* Data Modeling and Evaluation
* Conclusion and Recommendations

  # 4.Data Understanding

The data used in this project was provided by researchers at Zillow website. It consists of 14,723 rows and contains a small series of categorical features, as well as a large number of columns, each containing the median value of homes in a zipcode for a certain month. The months range from April 1996 to April 2018. The dataset includes features such as RegionID, RegionName (Zip code), City, State, Metro, CountyName, and SizeRank.

# 5.Data Preparation

To prepare the data for modeling and exploration, the pd.melt function was applied to transform the dataset from a wide format to a long format, resulting in a dataset with 3,901,595 rows and 11 columns. The data cleaning process involved handling missing values and checking for duplicates.

# 6.Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to uncover various patterns. The most popular state, city, and average profit margin per state were determined. Mean %ROI by zipcode and house value were also examined.

# 7.Data Preprocessing

During EDA, we noticed that the dataset as provided by Zillow comes in "wide format" and for our time series models to run, we had to convert it to "long format." A function was provided to do this. The top 5 zip codes based on %ROI were filtered, and data was grouped by date and zipcode, calculating the mean price for each group selecting from 2012. Home prices and monthly returns of each zipcode were plotted.

# 8.Data Modeling and Evaluation

The data was modeled using statistical time series models, such as ARIMA and SARIMA. The model's performance was evaluated using several metrics, such as Mean Squared Error (MSE) and Return on Investment (ROI).

# 9.Conclusion and Recommendations

We concluded that all the zip codes have an encouraging predicted price seeing as they are in the positive,apart from  the 85035 zip code.The investor can therefore decide to invest in zip codes 94804,94590,94601, and 85008 as they have a positive return on investment.




