# Title: Chicago Food Inspections

# Abstract
*A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?*

Food safety has been a question to be asked when eating out even before the taste of the restaruant. So how clean is your food when you are eating out in Chiago? Based on the dataset released by the City of Chicago, 


idea: 
goals: 
dataset: 

# Research questions
*A list of research questions you would like to address during the project.*

**Basic Questions:**
1. Is there a seasonal pattern for food hygiene of food establishments in Chicago? Are restaraunts generally cleaner in the winter than in the summer?
2. Is there a regional pattern for food hygiene? 
3. Which type of food establishments is the best? What is the ranking of the types according to cleaniness?

**Community-related Questions:**
4. For each zip-based region, is there a relationship between the cleaniness of food establishments and the quality of the region (average income, living cost, crime rate and etc.) ? Are wealthy regions overall cleaner than underdeveloped regions?
5. 9年内不同区域的卫生情况走势

**Causation-related Questions:**
6. 具体的卫生情况的那些comments的分析
7. For each violation, group by 'pass, pass with conditions and fail', which type of violation is the most incorrigible? Which are most easily-correctable? 
8. Is there a correaltion between the overall cleaniness condition of all restaruants and any health-related events happend in Chicago?

# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

**Chicago Food Inspections**
From https://www.kaggle.com/chicago/chicago-food-inspections
This information is derived from inspections of restaurants and other food establishments in Chicago from January 1, 2010 to the present. Inspections are performed by staff from the Chicago Department of Public Health’s Food Protection Program using a standardized procedure. 

The schema of the dataset contains relevant information such as type (categorical), risk level (categorical), zip code (categorical), 

*Data size: 230MB
*Format: .CSV

**Qulaity of zip-based region**
https://www.bestplaces.net/find/zip.aspx?st=IL&city=1714000
Here we established a self-constructed dataset, where the primary key is the zip code and we scrape data from the website above to find the crime rate, income status and health 

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific.
