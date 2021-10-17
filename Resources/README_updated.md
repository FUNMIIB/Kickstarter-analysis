# Kickstarting with Excel

## Overview of Project
**Background**
This project is to help louise who launched a crowdfunding campaign for her play _fever_ **and almost met her fundraising goal of _$10,000_** to understand the trend of different campaigns outcomes relative to their launch dates and their funding goals.

### Purpose
**Goal**
To know how different crowdfunding campaigns fared in relation to their launch dates and their funding goals
**Approach/Method**
Using **Excel** to analyse and visualize campaign outcomes based on their launch dates and their funding goals in the kickstarter dataset.

## Analysis and Challenges
**Overview**
The analysis involves the use of _pivot table_ and _graphing_ in **Excel** to organize, sort, and analyse the kickstarter data in order to understand the trend of different campaigns outcomes (**successful, failed, canceled**) in relation to their launch dates and their funding goals.

### Analysis of Outcomes Based on Launch Date
I created a new column named **Years** in the `Kickstarter_Challenge.xlsx` workbook and used the `Year()` function to extract the "Date Created Conversion" column. I created a pivot table from the Kickstarter worksheet and filtered the pivot table on "Parent Category" and "Years. The 
Pivot table looks like the image below
![Pivot_table_Outcome_Based_on_Launch_Date.png](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Pivot_table_Outcome_Based_on_Launch_Date.png). Using the pivot table, I generated a line chart that looks like the image below
[Line_chart_Outcome_Based_on_Launch_Date2](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Line_chart_Outcome_Based_on_Launch_Date2.png)
I then filtered the column label to show only "successful", "failed", and "canceled" as shown in the pivot table image below
[Pivot_table_TheaterOutcome_Based_on_Launch_Date](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Pivot_table_TheaterOutcome_Based_on_Launch_Date.png) and created another line chart without the "live" outcome shown in the image below
[Line_chart_TheaterOutcome_Based_on_Launch_Date](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Line_chart_TheaterOutcome_Based_on_Launch_Date.png)

### Analysis of Outcomes Based on Goals
Finally, I created a new sheet with a "Goal" column populated with dollar amount range to visualize the percentage of successful, failed, and canceled plays. I used the `COUNTIFS` function to collect the number of outcome data and also generated the percent outcome. The excel sheet is shown below
[Sheet_Outcome_based_on_Goals](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Sheet_Outcome_based_on_Goals.png)
line chart generated is shown below
[Line_chart_Outcome_Based_on_Goal](https://github.com/FUNMIIB/Screen-Shots/blob/main/Screen-Shots_2/Line_chart_Outcome_Based_on_Goal.png)

### Challenges and Difficulties Encountered
* Filters
  A few times during the "Outcome based on Goal" analysis, previous filters caused me some difficulties in getting expected results. 
    * How I overcame it
      I was able to proceed with analysis after I canceled the filters.
* Criteria-range: `COUNTIFS()` function
  I did not know how to correctly write the "criteria-range" syntax for dollar amount range. Less than 1000 and greater than 50,000 were easy but the ranges took me over 2 hours to figure out. 
    * How I overcame it
      I watched videos to see different examples and I finally got it to work.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
**Outcome based on Launch Date conclusions**
- Highest successful campaign happened in the month of May
- No campaign was canceled in the month of October

- What can you conclude about the Outcomes based on Goals?
**Outcome based on Goals**
- No fundraising campaign was canceled in the subcategory of "plays" 
- The highest number of **successful** and **failed** campaigns are in the goal range of $1000 to $4999.
- What are some limitations of this dataset?
- The organization and the structure of the dataset could be improved 
- What are some other possible tables and/or graphs that we could create?
- We could create a graph of outcomes based the different countries