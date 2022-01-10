# Module 1 Challenge - Analysis on Kickstarter data
# 1.	Overview of Project: 
The purpose of this analysis is to analyze the data and visualize campaign outcomes based on their launch dates and their funding goals and help Louise understand how different campaigns fared in relation to their launch dates and their funding goals.

# 2.	Analysis and Challenges: 

# Deliverable 1: Outcomes Based on Launch Date Chart
First, I started getting situated with the big picture, resizing columns to make sure I was able to visualize all the data properly. 
I filtered the column headers in case I needed to apply specific filters to better analyze the data and get to results and conclusions.
I also renamed the sheets and changed data formats where necessary.

Conditional Formatting
I have applied conditional formatting on the “F” column/”Outcomes” so it would be easier to visualize which plays were successful, failed, canceled or went live. 
Pivot Table
To better analyze this data, prior to creating the Pivot Table, a few steps were necessary.
First, I had to split the Category and Subcategory column into two distinct columns: "Parent category" and "Subcategory” so I could analyze the outcomes of each categories.
For that, I’ve used the "Text to Columns" function on the Data tab.
Second, I had to format the “Date Created” column and use “Year()” function to have a column with year per outcome.
Once the data was formatted and organized, I was able to select the data and create a Pivot Table, including as filters the “Parent category” and “Years” and then including the months at the rows labels. The result brought the count of the “successful”, “failed” and “canceled” per theater plays.
With that data organized on the Pivot Table, I was able to generate a pivot chart and save as image.

# Deliverable 2: Outcomes Based on Goals Chart
I have started creating a new sheet and relabeling it. 
In the first column I have included the Goals and its ranges below.
Whit that ready, I have started creating 12 different COUNTIFS for the 12 single intervals of the Goal. 
After that, I used the Replace function to replace “successful” to “failed” and, also “canceled” using the same formula for the Number of Successful, Number of Failed and Number of Canceled.
Once that was in place I used SUM() and calculated the percentages.
With that data in place, I was able to create a line chart that summarized the percentages of plays that were “successful”, “failed” and “canceled” based on the 12 goal ranges.
Lastly, I have saved the chart as an image.

# 3.	Results: 
•	What are two conclusions you can draw about the Theater Outcomes by Launch Date?
If we filter for only the “Theater” Parent Category, we will find that there were 839 successful theater Kickstarters. Which means that: more than half of the Theater campaigns - precisely 61% - were successful in meeting their goal.
Considering the Launch Dates, we could affirm that 53% of the successful theater Kickstarters have their launch dates between the month of April and August which gives an interesting insight for Louise to try to launch more of the campaigns between those months. 
•	What can you conclude about the Outcomes based on Goals?
When we filter for only the “Theater” Parent Category and “Plays” Subcategory, we find that more than half of total projects – precisely 66% of the projects that had their goal from less than $1,000 to $50,000 were successful.
We can also find that campaigns that had their goal from less than $1,000 up to $14,999 had a better chance of being successful. On the other hand, campaigns with goals between $20,000 and $34,999 failed. 
In this case we could suggest that Louise can focus her campaigns with goals that goes from less than $1,000 to $14,999 once they presented bigger chances of success. 

# •	What are some other possible tables and/or graphs that we could create?
One other possible pivot table would be:
Drag and drop the following:
Country and Parent Category to Filters
Years/Months to Rows
Outcomes to Columns
Outcomes to Values
With this one we could help Louise understanding which categories are more successful so she could focus more on those.
