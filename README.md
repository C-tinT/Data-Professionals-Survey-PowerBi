# Data Transformation and Dashboard

## Project Overview

The results of an actual survey (according to the author of this data source) applied to individuals working with data.
We will use Power Query to transform the data and then summarise it into an interactive Dashboard.

The final product will include a comparison between salary and job roles, gender pay distribution, as well as the level of happiness based on other variables.

## Transforming the Data

  Upon exploring the source data I've identified several columns where the values not standardised. Whether the survey form had little data validation or none at all, there were multiple answers that referred to the same category but had extra wording.
  
  For example, when asked about their job role, some respondents provided more than one answer in the same field. To make these cells workable I just replaced them with the first option after splitting the original column.
  
  Another example was the 'Current Yearly Salary' which contained pay brackets (due to the structure of the survey). This meant that we also had a string type of data.
The solution was to split the column by delimiter, get the limits of the pay ranges and then calculate the AVG in a new custom column. 

## The Dashboard Preview















Data Source: https://github.com/AlexTheAnalyst/Power-BI/tree/main/Power BI - Final Project.xlsx

## Conclusions

If there is data doesn't fit the general pattern of your report consider adjusting it or removing. In both cases think carefully about how this is going to affect the final report.


