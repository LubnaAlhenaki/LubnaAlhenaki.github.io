---
layout: post
title: Project1 :New York Subways Traffic Analysis
---





## Problem Statement 

WomenTechWomenYes (WTWY) is an international organizationthat aims to encourage more women to participate in the technology field. The organization hosts an annual gala at the beginning of summer in order to spread awareness towards their goal. With limited resources, they want to reach the maximum amount of people at the NYC subway stations to promote the gala and future events.

## Workflow
The following figure shows the workflow of our analysis


## Data Acquisition
In this project we used [MTA Turnstile Data](http://web.mta.info/developers/turnstile.html), NYC subways data for two months May and August 2019. There are 14 data elements, each elements is descripe [here](http://web.mta.info/developers/resources/nyct/turnstile/ts_Field_Description.txt).However, there are 378 Stations, 469 Units ,and 224 Scp’s.The following figure is a smaple of dataset.



## Data cleansing
● Removing white spaces in columns’ names.
● Handling Entries and Exits accumulation process
● Dealing with missing and negative val


## Feature Engineering and Selection
• Date and Time columns was combined into one column named (DATE_TIME).Also,Station, Unit,Scp combined into (STATION_UNIT_SCP) column.
• Hours, Months, Weekdays, and Weekends columns were created from Date and Time columns.
• LINE NAME, DIVISION, DESC , C/A columns were droped because it's not needed in our goal.


## Resource Description
For more details please viste [Project Resource](https://github.com/thisismetis/sa19_ds1/tree/master/student_work/project1/team4).
* Subway folder that contain the code file.
* Project-01 pdf file that describe the project in details.

