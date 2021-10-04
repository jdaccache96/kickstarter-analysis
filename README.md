# Kickstarting with Excel

## Project Overview

The objective of this analysis is to gather information on money raising campaigns and convert that into usable data for decision-making. The analysis shows which months bring in the most success for different categories of campaigns. 

### Purpose
	
The purpose of this analysis is to provide Louise with helpful information on campaigns in her same category. This allows Louise to compare her results to campaigns that launched in the same month as hers, as well. Most importantly, this data helps Louise and any other user choose the best fit month for their campaign, as well as an attainable goal for their category. 

# Analysis and Challenges
	
First, we had to clean the data. The date launched and the deadline columns used the Unix timestamp. Therefore, we added two columns formatted with short date to show the date launched and the deadline. 

Then, we created a pivot table which can be used to compare the amount of campaign successes, fails, and cancellations during each month. We can also filter for whatever year or parent category we want. This information helps us decide which month to start a campaign. For Louise, we filtered down the crowdfunding campaigns to only theater categories. 

[Image for Theater Outcomes by Launch Date](./Resources/Theater_Outcomes_vs_Launch.png)

For analysis of outcomes based on goals, we used the countif() function to compile the data we needed for the range of goals we watned to pull data for. We created columns for successful, failed, and cancelled cmapaigns and used the sumif() function to find the total projects in each campaign. After that, we created a double line chart to compare the percentage sucessful, failed, and cancelled campaigns per goal category. 

[Image for Outcomes Based on Goals](./Resources/Outcomes_vs_Goals.png)

We also used the measures of central tendency and measures of spread to look deeper in the data. Using that information, as well as the box and whisker plot, we can find a range of goals that were successful and could point out outliers. From what’s provided to us, we can now find an attainable goal for our campaign and use the remaining data to find a suitable month to start. 

### Analysis of Outcomes Based on Launch Date
	
One of the decisions Louise needed to make was a launch date for her campaign. To use the raw data, we had to convert the Unix timestamp columns into a short date format, which included the launch date and deadline of each campaign. From there, we created a pivot table that showed us the number of successful, failed, and cancelled theater campaigns for each month. 

Creating a line chart helped us visualize the impact May and June had on campaign success rates. Therefore, Louise will want to start her campaign in either May or June. 

### Analysis of Outcomes Based on Goals
	
Next, we wanted to see how well different goal ranges performed. In order to find the data we needed for this analysis, we had to use the countif() function to compile the number of successful, failed, and cancelled campaigns in each range of goals. Then, we used the sum() function to add up the total number of projects. 

We created three columns to represent the percentage successful, failed, and cancelled campaigns as a percentage of the total projects in that goal range. 
This data is very helpful, because we were able to input it into a line graph that compares the success and failure rates of each goal range. It’s clear that there was a higher success rate for any campaign under $20,000. However, the $35,000 to $45,000 range also showed a higher success than failure rate. 

### Challenges and Difficulties Encountered

I didn’t really have any trouble with the work. However, I did enjoy learning how to use the iferror() function, since I used to use another method of clearing the errors. I can see someone encountering trouble with pulling the data using the countif() function, since the ranges are tricky. The biggest challenge is just making sure your functions are pulling correctly and you double check your totals, since we only look at successful, failed, and cancelled, but not live campaigns. 

## Results
-	I concluded that Louise could start her campaign in either May or June, since both have a high number of successes. As well, they were the only two months that had over twice the number of successes as failures. 
-	The chart displaying outcomes based on goals shows us that the best chance at success is a campaign under $1000. However, anything up to $19999 shows at least a 50% success rate.
-	The dataset contains limitations, because we could look further into the data and check average contribution and amount contributors. For instance, a specific month might have received a high number of donors, but the donation amounts were smaller. Therefore, we can still possibly choose a different month or goal if Louise can adjust her campaign to gain higher donations. 
-	Other tables or graphs we could use could be a graph comparing number of donors per month and compiling same data for the outcomes based on goals. We also need to compare years, because one year might have had a higher success rate in certain months, but it’s different in another year. The data can tell us why these months failed, and we can have more options for our campaign. 
