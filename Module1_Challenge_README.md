# Kickstarting with Excel

## Project Overview
Louise's play *Fever* came close to its fundraising goal in a short amount of time. Due to these two variables of fundraising goals and time, Louise wants to analyze how other campaigns managed when considering launch dates and funding goals. Below is an image of various data collected for Louise's play *Fever*. Lousie had a goal of $2885; however, only $2485 was pledged. The fundraiser was launched on June 13, 2016 and had a deadline of July 11, 2016. Below is an analysis annd results of the data gathered and created. 

![Fever Play Data](https://github.com/Leung-Philip/Module-1-Challenge/blob/master/Resources/Fever_Play_Data.png)

### Purpose
Excel will be used to analyze the Kickstarter dataset and to provide visualizatons for Louise to better help determine her funding goals and launch dates. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![Theater Outcomes by Launch Date Pivot Table](https://github.com/Leung-Philip/Module-1-Challenge/blob/master/Resources/TheaterOutcomesbyLaunchDate_PivotTable.png)
![Theater Outcomes vs Launch Date](https://github.com/Leung-Philip/Module-1-Challenge/blob/master/Resources/Theater_Outcomes_vs_Launch.png)

A pivot table was created based on the original dataset. Parent Category and Years were set as Filters; Outcomes were set as Columns; Date (in the form of months) were set as Rows; and Count of Outcomes were set as Values.

A line graph with markers was created based on the pivot table. The X-axis represents the months and the Y-axis represents the count of the outcomes. 
All years (2009-2017) of the theater parent category were considered. Additionally, only fundraisers that were successful, failed, or canceled were considered. 

### Analysis of Outcomes Based on Goals
![Outcomes Based on Goals Table](https://github.com/Leung-Philip/Module-1-Challenge/blob/master/Resources/OutcomesBasedOnGoals_Table.png)
![Outcomes vs Goals](https://github.com/Leung-Philip/Module-1-Challenge/blob/master/Resources/Outcomes_vs_Goals.png)

A table of Goal ranges were created - from less than $1000 to greater than $50000. The ranges were in approxiamtely $5000 increments. A COUNTIFS function was used to determine the number of successful, failed, and canceled plays subcategory within each range. A SUM function was used to sum the total number of successful, failed, and canceled play in each range. Percentage successful, failed, and canceled columns were created by using a formula of number of successfull, failed, or cancelled divided by the total projects within each range. 

A line graph was created based on the goal ranges and percentage successful, failed, and canceled. The X-axis represents the goal ranges and the Y-axis repreesents the percentage.

All years (2009-2017) in the plays subcategory were considered. Additionally, only fundraisers that were succesful, failed, or canceled were considered. 

### Challenges and Difficulties Encountered
There were no difficulties encountered. However, a potential difficulty could be setting up the pivot table e.g. which variables would be in the columns and rows. Another difficulty could have been setting the rows to months given a date that did not separate the month, day, and year. Fortunately, there is an option in Excel to set the date to months when creating the pivot table.

## Results

### Conclusions for Outcomes based on Launch Date
On a seasonal basis, Spring and Summer seem to be the best months to launch a fundraiser. According to the data, the best month to launch a fundraiser is May, followed by June. 
Fundraisers generally do not get canceled; they either succeed or fail. 

Since successful and failed fundraisers increase and descrease similarly on a monthly basis, there is probably another variable that causes a fundraiser to succeed or fail. 

For Louise to have a successful fundraiser, it is recommended to launch in Spring or Summer. Additionally, more research is needed to determine what other variables would cause a fundraiser to succeed or fail.

### Conclusions for Outcomes based on Goals
The smaller the goal, the higher the percentage of success. The greater the goal, the higher the fail percentage. 

The exception is the goal ranges $35000-39999 and $40000-44999. These two goal ranges do not follow the trend and have a high percentage of success with a low fail percentage.

Approximately 51% of total projects had a goal range $1000-4999. This range had a successful percentage of 73%. If a goal this range was to increase by approximately $30000, the successful percentage only drops by 6%.

Louise should consider setting a fundraiser goal in the $35000-39999 and $40000-44999 ranges since there is a 67% percent chance of success and 33% chance of failing. 

### Limitations of this dataset
The data for Outcomes based on Launch date seem to be missing a key variable since successful and failed fundraisers increase and descrease similarly on a monthly basis. Whether it is included in the dataset or not, there is a vairable driving the increases and decreases similarly on a monthly basis. It provides a correlation between success and failed fundraisers per month, but does not mean that launching a fundraiser on a certain month will be successful or not. 

Similarly with the Outcomes Based on Goals data, a variable seem to be missing that could explain why fundraiseres had high percentage of success and low percentage of failure in the goal ranges $35000-39999 and $40000-44999. Again, this conclusion is just correlation. Choosing a fundraiser goal in the goal ranges of $35000-39999 and $40000-44999 will not always result in a successful fundraiser.

### Other possible tables and/or graphs that could be created
Based on Louise's play, she wanted to analyze how the fundraiser goal and launch date could play a role in a successful or failed fundraiser. According to *Fever's* data, it came up $400 shy of meeting the goal. This goal range has a 73% chance of success. However, the launch date and deadline consisted of 28 days. Another graph that could be utilzied is, Outcomes Based on Length of Fundraiser. This data, in combination with Outcomes Based on Goal ranges and Theater Outcomes by Launch Date, could help Louise meet her goal. 
