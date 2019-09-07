---
layout: post
title: Project1 :New York Subways Traffic Analysis
---





## 1. Problem Statement 

WomenTechWomenYes (WTWY) is an international organizationthat aims to encourage more women to participate in the technology field. The organization hosts an annual gala at the beginning of summer in order to spread awareness towards their goal. With limited resources, they want to reach the maximum amount of people at the NYC subway stations to promote the gala and future events.



## 2. Workflow
The following figure shows the workflow of our analysis
![Image test]({{ site.url }}/images/project1-4.png)



## 3. Data Acquisition
In this project we used [MTA Turnstile Data](http://web.mta.info/developers/turnstile.html), NYC subways data for two months May and August 2019. There are 14 data elements, each elements is descripe [here](http://web.mta.info/developers/resources/nyct/turnstile/ts_Field_Description.txt).However, there are 378 Stations, 469 Units ,and 224 Scp’s.The following figure is a smaple of the dataset.

![Image test]({{ site.url }}/images/project1-1.png)

## 4. Data Understanding and Cleaning

#### 4.1. Data cleansing
* Removing white spaces in columns’ names.
* Handling Entries and Exits accumulation process
* Dealing with missing and negative value


#### 4.2. Feature Engineering and Selection
* Date and Time columns was combined into one column named (DATE_TIME).Also,Station, Unit,Scp combined into (STATION_UNIT_SCP) column.
* Hours, Months, Weekdays, and Weekends columns were created from Date and Time columns.
* LINE NAME, DIVISION, DESC , C/A columns were droped because it's not needed in our goal.



## 5. Data Visualization

We grouped the dataset by STATION_UNIT_SCP and calculated the sum of its TOTAL_TRAFFIC column (total of Entries and Exits).Next, We plotted a line and bar charts using Matplottlib representing the top five crowded STATION_UNIT_SCP in NYC on Aug and May 2019 depending on the avrage of TOTAL_TRAFFIC.

The following figere shows the top five Stations based on Average traffic in May
![Image test]({{ site.url }}/images/project1-5.png)
The following figere shows the top five Stations based on Average traffic in Aug
![Image test]({{ site.url }}/images/project1-6.png)

The Figures below is a graph of avrage traffic per hours in weekends and weekdays. We concluded from the graph that rush hours in weekdays are the most crowded days unlike weekends.

![Image test]({{ site.url }}/images/project1-3.png)

![Image test]({{ site.url }}/images/project1-2.png)

## 6. Results




## 7. Resource Description
For more details please viste [Project Resource](https://github.com/thisismetis/sa19_ds1/tree/master/student_work/project1/team4). This repo contains the following:
* Subway folder that contain the code file.
* Project-01 pdf file that describe the project in details.

