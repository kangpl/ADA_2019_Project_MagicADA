# Guidebook for Opening a Restaurant in Chicago

***-- Insights from Dataset "Chicago Food Inspections" and beyond***

Team Members: Peilin Kang, Wan-tzu Huang, Futong Liu, Zhenyu Zhu

# Abstract
All successful businesses are alike; each unsuccessful business is unsuccessful in its own way. When it comes to the case of a restaurant, an unsuccessful one must have a deficiency of one or more critical factors, and a successful one on the contrary avoids every possible deficiency. That being so, can we find a universal pattern of critical factors that makes a successful restaurant? 

This project aims to explore the possible factors that affect the business of a restaurant in Chicago, IL based on the data collected from Chicago Department of Public Health, Yelp.com and regional information of each zip-based region. We would like to conclude insights for opening a new restaruant in Chicago by weighing factors such as its market positioning, cuisine type, shop front location, and especially give advices for restaurant hygiene and food safety. Ideally we can find a model to give a prediction for a new restaurant given these factors. 

The main datasets used in the project are `Chicago Restaurant Information in Yelp`, `Chicago Food Inspection` and `Community Qulaity of Zip-Based Region`. 


# Research questions
*A list of research questions you would like to address during the project.*

**Basic Questions:**

1. Is there a seasonal pattern for inspection results of food establishments in Chicago? How about a a regional pattern?
2. Which facility type is the best? What is the ranking of facility types according to cleaniness?

**Community-related Questions:**

3. Is there a relationship between the cleaniness of food establishments and the quality of the zip-based region (eg. average income, living cost, crime rate and etc.) ? Are wealthy regions overall cleaner than underdeveloped regions?
4. What tendency does the inspection result of each region exhibit during the recorded nine years?

**Inspection-comment-related Questions:**

5. Analyze the content of different types of Violations
6. For each violation, group by 'pass, pass with conditions and fail', which type of violation is the most incorrigible? Which are most easily-correctable? 
7. Is there a correaltion between the overall cleaniness condition of all restaruants and any health-related events happend in Chicago?

**If you want to invest in a restaurant in Chicago:**
For different grades restaurants, which factors are you needing to consider(categories, location, health and etc.)? Which health problems that are difficult to improve, you should try to avoid.


# Dataset
*List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.*

The primary datasets are `Chicago Restaurant Information in Yelp` and `Chicago Food Inspection`. We also combine data from `Community Qulaity of Zip-Based Region`.

**Restaurant Information in Chicago from Yelp**
<br>
Source: *https://www.yelp.com/search?cflt=restaurants&find_loc=Chicago%2C%20IL*
<br>
From Yelp, the well-know review webiste, basic information of each restaurant in Chicago has been scraped and saved to the file `ylep.csv`, as in the repsitory. In total, there are 7675 restaurants captured in Chicago area, which is almost the total number of restaurants that can possibly be found in Chicago. This dataset includes the restaurant name, address in Chicago, cuisine category, average rating, how many people have rated this restaurant and average price of a meal. We woud like to use the average rating to determine the success of a restaurant and figure out the influence of each factor on the rating. 

*Data size: 1.2MB*
<br>
*Format: .CSV*

**Chicago Food Inspections**
<br>
Source: *https://www.kaggle.com/chicago/chicago-food-inspections*
<br>
This information is derived from inspections of restaurants and other food establishments in Chicago from January 1, 2010 to the present. Inspections are performed by staff from the Chicago Department of Public Health’s Food Protection Program using a standardized procedure.\
This dataset contains information about each inspection, such as inspection date, inspection type, inpsection result, detailed comment for results and etc. Additionally, each inspection also records the information about the food establishment, such as the establishment's name, address, what type of food business it is doing and etc. We would like to join this dataset of the Yelp dataset by restaurant to observe the relationship between the hygiene of a retaurant and its rating.  
<br>
*Data size: 230MB*
<br>
*Format: .CSV*

**Community Qulaity of Zip-Based Region**
<br>
Source: *https://www.bestplaces.net/find/zip.aspx?st=IL&city=1714000*
<br>
56 zip codes
This small dataset contains information about the 56 zip-based region in Chicago. For each zip-based region, it includes the cost of living in the region, population, crime rate and etc. 
We aim to deduce from this dataset the quality of each region and attempt to correlate this region-based pattern with the region-based pattern of the quality of restaurants. 

*Data size: 56 pieces of information*
<br>
*Format: .CSV*


# A list of internal milestones up until project milestone 2   
We set up internal milestones for each week, and the group members will meet every Sunday night.  
**03.11.2017**:  
- Scrape Chicago restuarant information from Yelp to construct our own dataset.  
- Clean both the `Chicago Restaurant Information in Yelp` and `Chicago Food Inspection` datasets.  
- Find the ways to Merge the `Chicago Food Inspection` dataset into `Chicago Restaurant Information in Yelp` dataset.  

**10.11.2017**:  
- Analysis the newly merged dataset from different aspects to get preliminary findings, mostly based on the research questions listed above.  

**17.11.2017**:  
- Discuss the findings between teammates and explore the dataset further.  
- Explore ways to visualize our data.  

**24.11.2017**: 
- Have a nice visualisation and first results in notebook.  
- Discuss more detailed plan for future work based on the insights we get for the dataset.  

# Questions for TAa
- The number of Chicago restuarants we scraped from yelp is around 6500, is the size of the dataset large enough for us to make a project? 
- We will use the `Chicago Restaurant Information in Yelp` as the main dataset(scraped by ourself) and `Chicago Food Inspection` as an auxiliary dataset(provided dataset), is it ok for us to arrange datasets like this? 
- When we try to merge the `Chicago Food Inspection` dataset into `Chicago Restaurant Information in Yelp` dataset using restuarant name and part of the address, we found though sometimes they are the same restaurants, but the name and address will have silghtly difference in two datasets (for example, subway and subway restuarant, Av and Avenue). How can we deal with this problem? 
