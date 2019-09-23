---
layout: post
title: Project2: Movie Scraping and Regression Analysis
---

## 1. Objectives

WomenTechWomenYes (WTWY) is an international organizationthat aims to encourage more women to participate in the technology field. The organization hosts an annual gala at the beginning of summer in order to spread awareness towards their goal. With limited resources, they want to reach the maximum amount of people at the NYC subway stations to promote the gala and future events.



## 2. Workflow
The following figure shows the workflow of Predicting Movie Domestic Total Gross 
![Image test]({{ site.url }}/images/project2-1.png)



## 2.1 Scraping the Data
The data scraping was one of the most time consuming parts of this project because it’s difficult to navigate through the nested tables (the HTML). However, BeautifulSoup made it quite simple to grab the HTML and parse through it.

In this project I scraped from [boxofficemojo](https://www.boxofficemojo.com), I decided to start by scraping top of all  movies relased in 2018 so that I could build out my model. When I looked at the [page](https://www.boxofficemojo.com/yearly/chart/?yr=2018&p=.htm) that includes all movies that released on 2018. As a first step, I noticed that I need to collect all linkes of all movies then  go into each movie to collect the needed information. A lot of interesting information was captured in the table at the top of each movie page. The following figure is a smaple of strategy of scraping movies.

![Image test]({{ site.url }}/images/project2-2.png)

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

After completing the analysis and visualization, we recommend distributing the teams on the stations mentioned above ( depending on the month) at rush hours weekdays and late night in weekends. 

  


## 7. Resource Description
For more details please viste [Project Resource](https://github.com/thisismetis/sa19_ds1/tree/master/student_work/project1/team4). This repo contains the following:
* Subway folder that contain the code file.
* Project-01 pdf file that describe the project in details.


