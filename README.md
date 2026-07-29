# Data Transformation and Dashboard

## Project Overview

The results of an actual survey (according to the author of this data source) applied to individuals working with data.
We will use **Power Bi Desktop** to transform the data and then summarise it into an interactive Dashboard.

The final product will include a comparison between salary and job roles, gender pay distribution, as well as the level of happiness based on other variables.

## Transforming the Data

  Upon exploring the source data I've identified several columns where the values not standardised. Whether the survey form had little data validation or none at all, there were multiple answers that referred to the same category but had extra wording.
  
  For example, when asked about their job role, some respondents provided more than one answer in the same field. To make these cells workable I just replaced them with the first option after splitting the original column.
  
  Another example was the 'Current Yearly Salary' which contained pay brackets (due to the structure of the survey). This meant that we also had a string type of data.
The solution was to split the column by delimiter, get the limits of the pay ranges and then calculate the AVG in a new custom column.

**Data Source:** https://github.com/AlexTheAnalyst/Power-BI/tree/main/ Power BI - Final Project.xlsx

## The Dashboard Preview

![](https://github.com/C-tinT/Data-Professionals-Survey-PowerBi/blob/32c121f830feadaa465dcac68f75cd2195737cbc/Dashboard%20-%20Preview.png)

- A quick look reveals that 630 of professionals answered the survey. The average age was 30 and most of them were from US.

- The highest salaries were being paid to Data Scientists, followed at significant distance by Data Engineers and Data Architects.

- Gender pay seems to have a fair distribution 50.80% (women) and 49.20% (men), however one should pay attention to the total number of female participants (168). &#128521;

- The most frequent programming language is Python by far, used predominantly by Data Analysts.

- Finally the happiness gauges tell us that on a scale from 0 to 10 the participants' satisfaction with the Work/Life balance is at 5.74.
The satisfaction with the salary is at 4.27. Both genders have rated these parameters almost identically.


## Conclusions

- If there is data that doesn't fit the general pattern of your report consider adjusting it or removing. In both cases think carefully about how this is going to affect the final report.
- The analysis could be extended to other variables. I've only included a few due to the limits of my dashboard.
- As a consideration for future projects is that the survey is 4-5 years ago, so further analysis on fresh data could reveal interesting details about the current trends. 
