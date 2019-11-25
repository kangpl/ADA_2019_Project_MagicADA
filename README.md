### For Milestone 2: Our work is saved in project.ipynb.

# Insights from Chicago Food Inspections

Team Members: Peilin Kang, Wan-tzu Huang, Futong Liu, Zhenyu Zhu

# Abstract

Food hygiene has been a buzz word of the public and the society. How clean are the resaurants you are eating and what are the possible factors that are associated with food hygiene? 

This project aims to explore the possible factors that affect the cleaniness of a food establishment in Chicago, IL based on the data collected from Chicago Department of Public Health. We would like to find insights between food establishment cleaniness and time, location, risk level category and facility type. Furthermore, we analyse the violation comment of the inspector to find the relationship between the underlying banes and other factors (inspection type, facility type). Finally, we use restaurant rating, price and etc. collected from Yelp.com to get wider perspectives for analysing cleaniness.

The main datasets used in the project are `Chicago Food Inspection`, `Chicago Restaurant Information in Yelp` and `Community Qulaity of Zip-Based Region`.


# Research questions

### A. Inspection-Related Questions:
1. Time: Is there a seasonal pattern for inspection results of food establishments in Chicago? How about a a yearly pattern? What tendency does the inspection result of each region exhibit during the recorded nine years?
2. Region: Is there a relationship between the cleaniness of food establishments and the quality of the zip-based region? What is the distribution of cleaniness w.r.t. zips?
3. Risk Level: How does the risk level of a food establishment influence its cleaniness?
4. Facility Type: Which facility type is the cleaniest? What is the ranking of facility types according to cleaniness?

### B. Violation-Related Questions:
5. Inspection Type: What are the most frequent violations associated with a specific inspection type? How can we classify inspection types according to it?
6. Facility Type: What are the most frequent violations associated with a specific facility type? How can we classify the facility types? 
7. Regulation Rules: What are the regulation rules that have the highest occurence percentage and recurrence percentage? What are the high frequency key words associated with a regulation rule? How does its word cloud look like?

### C. Combine with Yelp:
8. Is there a clear correlation between the cleaniness of a restaurant with its average rating, cuisine type, average price and etc.? If yes, to what extent does it affect the cleaniness?


# Dataset

The primary datasets are `Chicago Restaurant Information in Yelp` and `Chicago Food Inspection`. We also combine data from `Community Qulaity of Zip-Based Region`.

**Chicago Restaurant Information in Yelp**
<br>
Source: *https://www.yelp.com/search?cflt=restaurants&find_loc=Chicago%2C%20IL*
<br>
From Yelp, the well-know review webiste, basic information of each restaurant in Chicago has been scraped and saved to the file `yelp.csv`, as in the repsitory. In total, there are 7675 restaurants captured in Chicago area, which is almost the total number of restaurants that can possibly be found in Chicago. This dataset includes the restaurant name, address in Chicago, cuisine category, average rating, how many people have rated this restaurant and average price of a meal. We woud like to use the average rating to determine the success of a restaurant and figure out the influence of each factor on the rating. 

*Data size: 1.2MB*
<br>
*Format: .CSV*

**Chicago Food Inspections**
<br>
Source: *https://www.kaggle.com/chicago/chicago-food-inspections*
<br>
This information is derived from inspections of restaurants and other food establishments in Chicago from January 1, 2010 to the present. Inspections are performed by staff from the Chicago Department of Public Health’s Food Protection Program using a standardized procedure.\
This dataset contains information about each inspection, such as inspection date, inspection type, inpsection result, detailed comment for results and etc. Additionally, each inspection also records the information about the food establishment, such as the establishment's name, address, what type of food business it is doing and etc. We would like to join this dataset of the Yelp dataset by restaurant to observe the relationship between the hygiene of a retaurant and its rating.

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
We set up internal milestones for each week, and group members will meet every Sunday night to update and split the work.

**03.11.2017**:  
- Clean both the `Chicago Restaurant Information in Yelp` and `Chicago Food Inspection` datasets.  
- Find the best way to join the `Chicago Food Inspection` dataset with `Chicago Restaurant Information in Yelp` dataset.  

**10.11.2017**:  
- Analyse the newly merged dataset from different aspects to get preliminary findings, mostly based on the research questions listed above.  
- Explore ways to visualize the findings. 

**17.11.2017**:  
- Discuss the findings between teammates and explore the dataset further.  
- Build a prediction model for a new restaurant given some basic information and outputs its likely business situation.

**24.11.2017**: 
- Have a nice visualisation and first results in notebook.  
- Discuss more detailed plan for future work based on the insights we get for the dataset.  

# Questions for TAa
- The number of Chicago restuarants we scraped from yelp is around 7600, is the size of the dataset large enough for us to make a project? 
- We will use the `Chicago Restaurant Information in Yelp` as the main dataset(scraped by ourself) and `Chicago Food Inspection` as an auxiliary dataset(provided dataset), is it ok for us to arrange datasets like this? 
- When we try to merge the `Chicago Food Inspection` dataset into `Chicago Restaurant Information in Yelp` dataset using restuarant name and part of the address, we found though sometimes they are the same restaurants, but the name and address will have silghtly difference in two datasets (for example, subway and subway restuarant, Av and Avenue). How can we deal with this problem? 
