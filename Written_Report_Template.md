# Kickstarting with Excel

## Overview of Project
A person named Louise sought to funraise money through Kickstarter for her play called *Fever*. It narrowly missed its fundraising goal albeit being up for only a short amount of time. We began with a dataset that contained a wide variety of statistics for over 4,000 different Kickstarter campaigns. 
### Purpose
The goal of this analysis is to help Louise understand how different campaigns performed in relation to their launch dates and funding goals. She ultimately wants to know how she can achieve the funding goal for one of her plays through a Kickstarter campaign.
## Analysis and Challenges
The analysis of this project was reletively straightforward. I thankfully didn't run into many challenges. One of them was not having used Excel's COUNTIFS() in a long time. It's probably easy to guess that this was an easy fix via the internet! A challenge that I didn't personally run into but others may have was being able to manipulate the charts almost soley using Excel's interface. I can imagine that there are people who had the same knowledge of using charts in Excel as I did but didn't process the interface the same way I did. My results are presented below.  
### Analysis of Outcomes Based on Launch Date
This analysis required filtering the "parent category" column to reflect only the "theater" campaigns. Using this, the outcomes column, and only the month part of the "date created conversion" column, I created a marked line chart to show the relationship between theater campaign launch months and outcomes (see below).

![alt text](https://github.com/mansal2487/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)


As you see above, theater Kickstarter campaigns were clearly most successful around the month of May. The number of failed theater campaigns around May is similar to the rest of the months.
### Analysis of Outcomes Based on Goals
This analysis first required using Excel's COUNTIFS() function to count the number of "successful", "failed", and "canceled" outcomes that had "plays" as their subcategories and whose goal fell within a certain range (which we were provided with). I then found the percentage of "successful", "failed", and "canceled" outcomes for each of these ranges and plotted those numbers versus each range (see below).

![alt text](https://github.com/mansal2487/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


Here we have multiple data points that are worth noting. For the range of "less than 1000", the success rate is about 60% higher than the failure rate. On the other hand, the range of "25000 to 29999", the failure rate outweighs the success rate by about 60%. For the ranges of "35000 to 39999" and "40000 to 44999", both success rates were about 30% higher than the failure rates. For the range of "45000 to 49999", we see the biggest discrepancy with the failure rate beating the success rate by almost 100%.
### Challenges and Difficulties Encountered
As I discussed above, I didn't run into many challenges. I would like to go back and analyze this situation further to discover more relationships and possibly new conclusions.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
I would recommend to Louise that the next time she begins a Kickstarter campaign for something theater related that she does so around May. I would also recommend not starting it December as this month saw the lowest number of successful theater campaigns.
- What can you conclude about the Outcomes based on Goals?
First and foremost, I would recommend steering clear of setting a fundraising goal of $45,000 or more as the success rate is extrememly low. Depending how much money Louise is seeking, I would pursue a goal of less than $1,000 or between $35,000 and $44999" as those two had the highest success rates.
- What are some limitations of this dataset?
One limitation of this dataset is that we are unable to drill down on the donations from backers. It is easy to get the average donation per backer, but that doesn't tell us, for example, if 99% of campaign's goal was funded by a single person. This skews the credibility of the terms "successful" and "failed".
- What are some other possible tables and/or graphs that we could create?
Something I'd like to create is a table that, for each campaign, shows the difference between the goal and pledge amount. I would then like to take these amounts and create a reasonable amount of ranges with them. Using that I'd create a graph that shows the relationship between each range and the number of respective "successful" and "failed" campaigns.
