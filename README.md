# Insights from Chicago Food Inspections

Team Members: Peilin Kang, Wan-Tzu Huang, Futong Liu, Zhenyu Zhu

# Abstract

Do you live in Chicago currently? Have you ever wondered whether the place you dine out with a friend on Friday night is really clean and conform the hygienic standards? Or are you planning a visit to Chicago this coming holiday and wonder if it is really safe to try out the local cuisine at the random place without having the risk of gut-bombing food sickness that will ruin your vacation? 

This project aims to explore the possible factors that affect the cleaniness of a food establishment in Chicago, IL based on the data collected from Chicago Department of Public Health. We would like to find insights between food establishment cleaniness and time, location and facility type. Futhermore, we scrutinize how life expectacny and crime of each community relate to food inspectioni results. Finally, we use restaurant price, cuisine type, etc. collected from Yelp.com to get a wider perspective for analysing cleaniness.

At the end of the project, we hope that we can enlighten you with some useful suggestions on how to safely dine out in Chicago and more importantly some ideas on WHERE to eat, WHEN to eat and WHAT to eat in Chicago.


# Research questions

### A. When?
1. Is there a seasonal pattern for inspection results of food establishments in Chicago? 
2. How about a a yearly pattern for inspection results? What tendency does the inspection result of each region exhibit during the recorded nine years?

### B. Where?
3. What is the distribution of inspection results over each community of Chicago? Is there a relationship between the cleaniness of food establishments and the quality of life of each community?
4. Which facility type is the cleaniest? What is the ranking of facility types according to cleaniness?

### C. What?
5. What cuisine type is the most hygienic? Is there a clear relationship between the cleaniness of a restaurant's cuisine type?
6. What price does a hygienic meal cost? Does the price of a restaurant influence its hygiene condition?


# Dataset

The main datasets used in the project are `Chicago Food Inspection`, `Chicago Crime Records` and `Life Expectancy in Chicago` and data collected from Yelp.com.

**1. Chicago Food Inspection**
<br>
Source: *https://www.kaggle.com/chicago/chicago-food-inspections*
<br>
This information is derived from inspections of restaurants and other food establishments in Chicago from January 1, 2010 to the present. Inspections are performed by staff from the Chicago Department of Public Health’s Food Protection Program using a standardized procedure.\
This dataset contains information about each inspection, such as inspection date, inspection type, inpsection result, detailed comment for results and etc. Additionally, each inspection also records the information about the food establishment, such as the establishment's name, address, what type of food business it is doing and etc. We would like to join this dataset of the Yelp dataset by restaurant to observe the relationship between the hygiene of a retaurant and its rating.

*Data size: 230MB*
<br>
*Format: .CSV*


**2. Chicago Crime Records**
<br>
Source: *https://data.cityofchicago.org/Public-Safety/Crimes-2019/w98m-zvie*
<br>
This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that occurred in the City of Chicago from 2001 to present. Data is extracted from the Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system.\
Here we aim to find possible relationship between the food inspection results in a specific area and the number of crimes in that area. Therefore, we only care about the time and location of a specific crime record, and hence we only use a subset of the columns in Chicago Crime Dataset: ID(its primary key), Year, Block, Community Area, Latitude, Longitude.

*Data size: 1.66G*
<br>
*Format: .CSV*


**3. Life Expectancy in Chicago**
<br>
Source: *https://www.chicagohealthatlas.org/indicators/life-expectancy*
<br>
This dataset contains information about the life expectancy in each community in Chicago, as well as aggregated information for each ethinicity group and the whole city of Chicago.
We aim to deduce from this dataset the quality of each region and attempt to correlate this region-based pattern with the region-based pattern of food inspection results of restaurants. 

*Data size: 165B*
<br>
*Format: .xlsx*


**4. Chicago Restaurant Information on Yelp.com**
<br>
Source: *https://www.yelp.com/search?cflt=restaurants&find_loc=Chicago%2C%20IL*
<br>
From Yelp, the well-know review webiste, basic information of each restaurant in Chicago has been scraped and saved to the file `yelp.csv`, as in the repsitory. In total, there are 7782 restaurants captured in Chicago area, which is almost the total number of restaurants that can possibly be found in Chicago. This dataset includes the restaurant name, address in Chicago, cuisine category, average rating, how many people have rated this restaurant and average price of a meal. We woud like to use the average rating to determine the success of a restaurant and figure out the influence of each factor on the rating. 

*Data size: 1.2MB*
<br>
*Format: .CSV*


# Datastory

Website: https://holykhala.github.io/

Please use Safari for optimal user experience. If you are a chrome user, please do refresh your page when anything abnormal happens.

# Contribution 
Wan-Tzu: Writing up the data story, plotting graphs for data analysis;\
Peilin: Data cleaning, preliminary data analysis;\
Futong: Anlysing plotted graphs, exploratory data analysis;\
Zhenyu: Data collection, website of data stroy construction.
