# Kickstarting with Excel

## Overview of Project
This project uses Excel as the Data Analytics tool to visualize a dataset that will 
require some data analysis, manipulation and ultimately visualizations.  The visualizations include
line charts to see the successful, failed and canceled campaigns for specific criterias.

My client, Louise, achieved her fundraising goal quickly and is interested in 
seeing how other campaigns did with respect to their launch dates and funding goals.

I will be using the "Kickstarter" dataset to visualize my client's interests.

### Purpose
The purpose of this project is to produce two (2) visualizations that illustrate campaign outcomes using;
- outcomes and launch dates 
- outcomes and fund raising goals

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Using the Kickstarter dataset, this analysis included the creation of a Pivot table to illustrate the 
monthly successful/failed/canceled outcomes filtered on the years and parent category.  
The visualization for this analysis included the creation of a Line Chart.  
See the image file named "Theater_Outcomes_vs_Launch.png" in the resources folder.  

### Analysis of Outcomes Based on Goals
Using the Kickstarter dataset, this analysis included the creation of a Line Chart to illustrate the 
percentage of successful/failed/canceled outcomes based on the funding amounts for the "plays" subcategory.  This visual
displays all successful/failed/canceled outcomes percentages that fell into a specific funding goal range.  The visualization
for this analysis included the creation of a Line Chart.
See the image file named "Theater_Outcomes_vs_Launch.png" in the resources folder.  
The visualization for this analysis included the creation of a Line Chart.  
See the image file named "Outcomes_vs_Goals.png" in the resources folder.  


### Challenges and Difficulties Encountered
The analysis revealed that the launch date was not readable.  It was discovered to be in a Unix format.  
To resolve this challenge the following was completed;
- Copied the "launched_at" column" to a new column named "Date Created Conversion".
- Applied a function to each "Date Created Conversion" row. Example: =(((J2/60)/60)/24)+DATE(1970,1,1), J2 represents data from the "lauched_at" column.
- Created a new colmn named "Years" to the the year "only" from the "Date Created Conversion" column.  
The Excel Year() function was used to capture the year "only" from the "Date Created Conversion" column

## Results

### Two (2) conclusions can be drawn about the Outcomes based on Launch Date:
* There are more successful campaign outcomes than failed and canceled outcomes
* There was a spike of successful campaign outcomes in May

- A distint conclusion about the Outcomes based on goals:
* The goals in the range of 45000 to 49999 failed 100% of the time.

- Some limitations of the this dataset include;
* The "name" and "blurb" columns seems to suggest a campaign name and description; however, the data for does not appear to be accurate.  This information
would seem to deliver a more description about the campaigns and offer a different story.

- Some other possible tables and/or graphs are;
* A Line chart of the "ALL" Parent Categories to visualize their outcomes.
* A Pie chart of the top five (5) successful Parent Categories.
* A Line chart of the "ALL" Parent Categories to visualize their their goals.
* A Pie chart about the outcomes based on country would also appear to be helpful.

