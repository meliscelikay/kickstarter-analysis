# kickstarter-analysis
Excel project for analyzing kickstarter date
# Kickstarting with Excel

## Overview of Project
On this project, I used Kickstarter dataset for Louise’s play Fever to analyze the effectiveness of different campaigns in relation to their launch dates and whether they achieved funding goals or not.  


### Purpose
The purpose of this project is to understand and gain knowledge of how each campaign, specific to plays, performed regarding to launch dates and funding goals. 


## Analysis and Challenges
Before analyzing the results, I had to organize the dataset into category and subcategories. This additional step allowed me to group parent category of theater with its subcategory of plays in separate columns which provided the basis for more detailed analysis. 

[Kickstarter Challenge](https://github.com/meliscelikay/kickstarter-analysis/blob/6768f2238b419a2130bcc9fbe53d342dac456c75/Kickstarter_Challenge.xlsx)

### Analysis of Outcomes Based on Launch Date
The objective of this analysis is to observe the outcomes of theater campaigns which can be divided into three main categories: successful, failed, and canceled based on their launch date. Before analyzing the results, I had to take additional steps to breakdown the data. Initially, I had to create a new `Years` column, to extract the year from the `date created conversion` column, in order to highlight when the campaigned was launched. Next step, I created a pivot table in a new worksheet using the entire dataset.  Adding `parent category`, `years` to filters, `date created conversion` to rows, and `outcomes` to columns and values. This helped me create a pivot chart which can be further modified by removing the outcomes of live campaigns, limiting rows to show the months, and filtering the parent category to show just the `theater`. I used a line chart to illustrate the outcomes based on their launch month which made the pivot table data more visually pleasing and easier to understand.

![Resources/Theater_Outcomes_vs_Launch](/Resources/Theater_Outcomes_vs_Launch.png)   

### Analysis of Outcomes Based on Goals
The objective of the Goals analysis is to observe the percentage of successful, failed, and canceled plays in regard to funding goal amounts. This could not be done directly so I took these additional steps. Initially, I created 8 columns to hold: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled in a new worksheet. In the Goal column, create 12 rows from less than $1000 to more than $50,000. I used COUNTIFS function to show the outcome and goal data for `plays` subcategory to illustrate the number of successful, failed, canceled campaigns based of goal range. I used the SUM function to reach the Total Project of Number Successful, Number Failed, Number Canceled. Upon calculating the percentage of successful, failed and canceled projects, I added a line chart to display the data. 

![Resources/Outcomes_vs_Goals](/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
I encountered a few challenges during this project, the main one was sorting and arranging the pivot table fields. It took me some time (constant back and forth) to organize the filters, rows, columns, and value fields in order to create the data which would clearly summarize and presented the outcome of the campaigns. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The launch month of a theater campaign played a significant factor in its success or failure. It is clear that May and June campaigns were the most successful. The May campaign resulted in 111 successful, 52 failed, and 3 canceled. It is also very clear that the campaigns launched in October, November, and December have a low success rate, data shows these months have much higher fail and cancel rates. 

- What can you conclude about the Outcomes based on Goals?
Data clearly showed campaigns with goals less than $5,000 were more successful compared to larger goal amount campaigns. We see a 73% to 76% success rate for campaigns with less than $1,000 up to $4,999. 

- What are some limitations of this dataset?
The most significant limitation of the dataset used in this project was the lack of further details related to `plays`. Although the theater data was abundant, there was only 1065 data points on `plays`. More in-depth analysis can be performed if the overall data contains more subcategories with finer details. It would also be beneficial if we had more source data from other parties in addition to Kickstarter. More and wide-ranging data can offer better visibility and allow further analysis. 

- What are some other possible tables and/or graphs that we could create?
Although limited in some subcategories, Kickstarter campaign data can still provide more insight. There are 8 main categories and 36 subcategories left unexplored, perhaps further dive into these can yield more analysis. 
