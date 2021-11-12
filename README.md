# BST260project

This is our project Repsitory
BST 260 Project proposal

Team Members
Aravind Menon
Bina Choi
Zsu Zsu Chen
George Goshua

Title: Factors affecting housing inflation costs in metropolitan and suburban Boston during the COVID-19 pandemic

Background and Motivation:
Increases in real estate prices were seen across the country over the course of the COVID-19 pandemic, with the Case-Shiller U.S. National Home Price Index showing an 18.6% growth in housing prices over the course of September 2020 to 2021 (https://www.whitehouse.gov/cea/blog/2021/09/09/housing-prices-and-inflation/ ). Some factors contributing to this trend included both COVID-related and unrelated factors, such as: lower lending interest rates, changes in migration from urban to suburban areas or smaller cities given an increase in remote working (https://www.nber.org/papers/w26948), millennials aging into homeownership (https://www.vox.com/22264268/covid-19-housing-insecurity-housing-prices-mortgage-rates-pandemic-zoning-supply-demand), an increase in second-home buying (https://www.federalreserve.gov/econres/notes/feds-notes/housing-market-tightness-during-covid-19-increased-demand-or-reduced-supply-20210708.htm), and a variety of other factors (https://www.cnbc.com/2021/03/12/housing-market-covid-one-year-anniversary.html). 

We wanted to examine how the real estate prices in and around Boston were affected during the last four years. Given that Boston is a huge healthcare hub with some of the leading hospitals, pharmaceutical, and biotech companies, its housing market is more likely to be impacted by COVID-19 trends than other cities. Thus, it is a good model city to study the pandemic-related factors affecting housing inflation. Furthermore, given that Boston has the 4th most number of colleges in the US, trends in housing markets during the COVID-19 pandemic were likely to be affected by the 2021 influx of college and graduate students who in 2020 were learning remotely. 

In addition to the effect of the pandemic, we also wanted to explore other factors that may have affected the property prices. We want to contrast how price inflation varies according to neighbourhoods, their area deprivation index, school rating, air quality index (AQI), proximity to medical centers, etc. We believe that this would allow us to see the local impact of property price inflation that has been happening across the country. 


Project Objectives:
Objective 1: To assess the actual house sale price trend in real estate units from 2017 to 2021, with special attention to the years of the COVID-19 pandemic (2020-2021) and compare this to property value assessment data available from the Analyze Boston website (https://data.boston.gov/).  We plan to look at the actual selling price of various units from different Boston neighborhoods through a real estate database (i.e., Zillow, Redfin, or Trulia) and compare it to the City of Boston home assessment prices to see the divergence in the values that could be attributable to property price inflation.

Objective 2: Utilizing regression models based on property data from pre-pandemic (2017-2019) and pandemic (2020-2021) years, we will predict the possible change in housing prices for different metropolitan and suburban regions of Boston in 2022 given 1) there is no further COVID-19 surger and 2) there is another COVID-19 surge.

Objective 3: To assess for factors that affect inflation of property price beyond COVID-19, including sociodemographic (i.e., neighbourhood, ADI https://www.neighborhoodatlas.medicine.wisc.edu/ ), facilities (i.e., proximity to medical center https://data.boston.gov/dataset/hospital-locations, school district ratings https://www.niche.com/k12/search/best-school-districts/t/boston-suffolk-ma/) and environmental data (i.e., air quality index).


What Data: 
The primary data regarding the actual value of the property prices will be obtained through the city of Boston property assessment database available at: https://data.boston.gov/dataset/property-assessment for the years of 2017-2021. We plan to tag data with address being the unique identifier or if data is not available at such a granular level, zip code. Real world property closing price data will be obtained through web scraping from publicly available property listing websites including Zillow/Redfin/Trulia for the same time period.

We then plan to compare the differences in real estate prices across different neighbourhoods and find factors that may be contributing to the assessed and final selling price. Additional data inputs on crime, AQI, ADI and school districts will be scraped from online databases. 


Design Overview: 
Objective 1: Our main outcome for this objective is to compare if there is a statistically different amount of housing price inflation in the years before (2017-2019) and during the pandemic (2020-2021). Housing price inflation will be defined as the difference in actual sale price and property assessment value after adjusting for the property assessment value.  We will use linear regression models to compare these differences in houses sold from 2017-2019 to those sold in 2020-2021 after matching by property square footage, number of bathrooms, and parking if this data is available. A secondary analysis will be to compare across different Boston neighborhoods.

Objective 2: Our main outcome for this objective is to accurately predict housing prices in 2022 in the case a COVID-19 surge were and were not to occur. Since our outcome is a continuous variable, we will explore regression models including linear regression, kNN, decision trees, and random forest.

We will use linear regression to model property price trends in 2017 to 2019 to create a prediction model for housing prices if no further COVID-19 surge occurs in 2022 for the different metropolitan and suburban regions of Boston. We will create similar models for 2020-2021 to create a prediction model for housing prices if there is another COVID-19 surge in 2022. A sensitivity analysis will also be conducted with the inclusion and exclusion of 2020 data given Boston social distancing protocols which could have temporarily interrupted the housing market. 

Objective 3: We will use multiple linear regression models to explore if other factors such as neighborhood sociodemographics (defined by ADI), school districts, and air quality may contribute to house price inflation.

For our final product, we plan to create a data visualisation platform (using RShiny) to create an interactive map that will allow users to visualize differences in housing prices across the years of 2017-2021, see projected changes in the year 2022 given if a COVID-19 surge were or were not to occur, and see visualizations of regional differences in other sociodemographic and environmental factors that may be contributing to housing price inflations in the neighborhoods of metropolitan and suburban Boston.

Schedule/ TImeline
 
With overlap in dates
11/8 - 11/21: Web scraping and data base consolidation (Aravind and Zsu Zsu)
11/22 - 12/5: Model building and testing (Bina and George)
11/29 - 12/12: Data visualization (all)
12/6 - 12/12: Work on screencast and website (all)




