# Kickstarting with Excel

## Overview of Project

### In this project we were given crowd funding data to help Louise fund a play she has written. The purpose of the project was to help Louise determine if there are specific factors that make a campaign successful. Because her own play did not meet its goal in a short amount of time, she would like to see how the other campaigns fared. Specifically, she wants to know if there was any relation between the launch dates and the funding goals that made a campaign successful. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In the Outcomes Based on Launch Date sheet we analyzed the campaign outcomes based on the month they launched. This analysis is important because Louise’s play Fever did not meet its goal and she had a short amount of time to achieve her fundraising goal. To begin this analysis we will need to add a new column in the kickstarter sheet labeled “Years”. I then used the Year() function by placing the “Data Created Conversion” data in the function to output the correct year the campaign started. ![This is an image](<img width="453" alt="Screen Shot 2021-10-01 at 10 12 46 PM" src="https://user-images.githubusercontent.com/91295921/135741549-4aa12521-a1d7-49b3-b507-57bcb8a1340c.png">)

 
After the year column is filled out, I created a pivot table from the Kickstarter sheet. In the pivot table I used the “Parent Category” and “Year” as the filters for the table. The “Data Created Conversion” was used to populate the rows and the “Outcomes” field is summarized by “count” to display the data. “Outcomes” is also used in the Columns field. 
 
After I created the pivot table, I used the Column filter to only display “successful”, “failed”, and “canceled” data. 
 
The next step I took was filtering the “Parent Category” by clicking on the filter button in cell (B,2) and then choosing “theater” to only display theater campaigns by month. 
 
After filtering the “Parent Category” I sorted the outcomes in the pivot table by clicking the “Descending” button in the column filters to show the “successful” campaigns first and “canceled” campaigns last. 
 
The last step in this analysis is creating the line chart. To create the line chart I selected the entire sheet and then clicked on “insert” in the toolbar. From there I selected the line chart option to create the chart. 
 

### Analysis of Outcomes Based on Goals
The Outcomes Based on Goals sheet is an analysis of the campaign fundraising goals. In this analysis I used more formulas than the “Theater Outcomes Based on Launch Date” analysis. This analysis required much more attention to detail in order to make sure the formulas were correct and to make sure I wasn’t missing any steps. The first 
 

### Challenges and Difficulties Encountered
The biggest challenge I ran into during this project was in trying to display the correct line graph for the Outcomes Based on Goals analysis. When I create the line chart, I was getting a very different result from the chart shown in the challenge assignment. I initially thought it was because I needed to adjust the data selected in the chart, but the data selected was correct and I was still getting a different result. I then retraced my steps and began carefully going through the steps again to see if there was anything I had missed. After reviewing each step, I realized that there was one thing I was missing in my data. I had forgotten to filter it by plays. I had figured out what was missing but I wasn’t sure how to filter the data to only display the plays. After trying a few things with the formula I was able to filter it correctly by adding Kickstarter!$R:$R,"plays" at the end of the formula. 

## Results

- **What are two conclusions you can draw about the Outcomes based on Launch Date?** One conclusion I had from the Outcomes based on Launch Date analysis was that play writers like Louise will have a higher chance of successfully hitting their fundraising goal in the months of May and June. These months have the highest number of successful campaigns compared to the rest of the year. Another conclusion I made is that play writers should avoid trying to fundraise a play during the month of December because it has the lowest number of successful campaigns and the least number of total campaigns. Meaning theater fundraising campaigns aren’t as successful in the month of December compared to the rest of the year. 

- **What can you conclude about the Outcomes based on Goals?** The Outcomes based on Goals analysis shows that most of the fundraising campaigns had a goal that was less than or equal to $4,999. The line chart also shows that campaigns with a goal of less than or equal to $4,999 had a higher percentage of successful outcomes than the rest of the goals. Based on this data we can conclude that plays will have the best chance to hit their fundraising goal if their goal is less than or equal to $4,999. 

- **What are some limitations of this dataset?** Some of the limitations of this dataset are the 

- **What are some other possible tables and/or graphs that we could create?** A table that I thought about creating a pivot table that shows the outcomes vs country. This table would analyze the campaign outcomes based on the country. Louise would be able to use this table to see how campaigns fared in other countries and if it makes a difference in where you are launching your campaign. Most of the data is from the US and Great Britain so we could filter out the rest of the countries to see if there is a difference between these two countries. To visualize this data we could use a bar graph which in this case is more effective in showing the results of this table than using a line graph. Below is an example of what this table would look like, including the bar and line graph. In the example below the bar graph is easier to digest and understand while the line graph looks like it’s missing something.
