# Kickstarter-analysis
performing analysis on Kickstarter data to uncover trends.
## Overview of Project: 
The purpose of this project is to summarize the data by creating line chart. This also help Louise find easily the theater outcomes by Launched date and outcomes based on goals by looking at the pivot table and graphs. This visually process outcomes at a glance will be very useful for her past campaigns.. This would help her excute future campaigns that will yeild successful results. 
## ANALYSIS
# Analysis of outcomes based on launch date:
First, I created a pivot table for theater outcomes by launch date. Click on Insert and then click pivot table. Select the range and choose a new work sheet to create a pivot table. I filtered the parent category and years. Outcomes in my column, months in my rows and outcomes in my value. Chooses a descending order for my row label by clicking the arrow on row labels. 
Count of outcomes	Column Labels				
Row Labels	successful	failed	canceled	Grand Total	
 and filter the parent category for theater.
Parent category	theater	
Years	(All)	
Once I have the pivot table ready I can create the line chart by clicking Insert and choose line chart. The chart has a box in center says, add Text. Click on it and name the line chart “Theater Outcomes” and save it as Png in Microsoft paint.
![Theater_Outcomes_vsLaunch png](https://user-images.githubusercontent.com/107155888/173200057-512cda31-b433-42df-bb1b-8e2a3314369a.png)
# Analysis of outcomes based on goals:
First, I created the new sheet and set my goal ranges in a first column and then named my B through H column
Goal	Number Successful	Number Failed	Number Canceled	Total Project	Percentage Successful	Percentage Failed	Percentage Canceled	
Percentage Failed	Percentage Canceled	
To find the number of successful in goal range less than 1000 I used a COUNTIFS formula =COUNTIFS(kickstarter!D:D,"<1000",kickstarter!F:F,"Successful",kickstarter!R:R,"PLAYS")
Let’s break the formula
kickstarter!D:D : This means we are searching in the Kickstarter sheet goal column D and finding the result in the same column.
"<1000", This is our goal range. We are only interested in less than 1000 goal ranges.
kickstarter!F:F,"Successful”: This time we are looking in Kickstarter sheet  outcomes which is our column F and we are only interested in successful campaigns.
kickstarter!R:R,"PLAYS": This one tells excel we want only plays in our Subcategory column.
Copy and paste the COUNTIFS formula in our Number failed and Number canceled columns and just change the goal ranges in each row. Also, change the outcomes failed and canceled.
To find the percentages of our outcomes I used a round formula =ROUND (Total projects/Number outcomes*100,0). Zero tells we want no decimal. After using the round formula, we have our outcomes based on goals table ready. 
Let’s create a line chart now. First select the percentage columns F, G, AND H) and click on Insert and click on a line chart. Click on the add text in your chart and name the chart “Outcomes based on goals”. Now right click on a chart and click select data. I chose my goals to be my X-axis and percentage outcomes as my Y-axis based on the instructions.
 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/107155888/173199986-8a3e1776-5a69-43c9-8255-795221226e62.png)
# Challenge:
My challenge was to find the number of Successful, failed, and canceled by using COUNTIFS formula in outcome based on Goals table. I didn’t know how to set Goal range into COUNTIFS formula. The video is given in Module 1 challenge as a hint for COUNTIFS function helped me a lot. The video instructions are quicker and easier to follow.
## Results.
# Conclusions of Theater Outcomes by Launch Date:
The number of Successful theater campaign is much higher in the month of May.
There are only 37 Canceled theater campaign out of total 1,369 theater campaign. The total number of Success theater campaign is 839. Which is much higher than the other two outcomes (failed and Canceled).
# Conclusion of Outcomes based on Goals:
If we look at the Outcome based on goal chart. It shows up there’s 0% canceled campaign plays based on our Goal ranges.
Goal range 45,000 to 49,999 shows that there’s a 100% of failed campaign plays.
limition was only looking at the "plays" subcategory. While I wanted specific insights from the "plays" campaigns, it also would be helpful to compare that information to all campaigns on kickstarter. 
# Recommendations:
What are some other possible tables and/or graphs that we could create? We could also find the outcomes based on other columns such as Backers Count. Some possible metrics include (1) success rate per category/subcategory, (2) median, max, and min funding goal/target per category/subcategory, (3) median, max, and min of average donation per category/subcategory. We could also create the Bar chart of theater outcomes by launch date. Also, pie chart can be created to see the results of our outcomes.
