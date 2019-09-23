---
layout: post
title: Project2 :Movie Scraping and Regression Model
---



## 1. Objectives



In fact, the film industry is a significant player in the global economy.  In this project, I try to answer the question, which factors, if any, contribute to the success of films at the box office that will help business area.The major goal is to predict a domestic total gross value by using a linear regression model.The main objectives of this project are:

* Using BeautifulSoup to scrape web data (must have good knowledge in HTML)
* Using Statsmodels and Scikit-learn to build linear regression model
* Using power transformation to variables in order to create a better model
* Experiment between Lasso, Ridge, and Elastic Net to regularize the models (solve overfitting problem)
* Utilizing cross validation to build better model during sampling process



## 2. Workflow
The following figure shows the workflow of Predicting Movie Domestic Total Gross 
![Image test]({{ site.url }}/images/project2-1.png)



### 2.1 Scraping the Data
The data scraping was one of the most time consuming parts of this project because it’s difficult to navigate through the nested tables (the HTML). However, BeautifulSoup made it quite simple to grab the HTML and parse through it.

In this project I scraped from [boxofficemojo](https://www.boxofficemojo.com), I decided to start by scraping top of all  movies relased in 2018 so that I could build out my model. When I looked at the [page](https://www.boxofficemojo.com/yearly/chart/?yr=2018&p=.htm) that includes all movies that released on 2018, as a first step, I noticed that I need to collect all linkes of all movies then  go into each movie to collect the needed information. A lot of [interesting information](https://www.boxofficemojo.com/movies/?id=grinch2017.htm) was captured in the table at the top of each movie page. The following figure is a smaple of strategy of scraping movies.

![Image test]({{ site.url }}/images/project2-2.png)

At the end of this step, 879 movies and 8 features were collected then I saved all these information into CSV file. The featuers are Title, Domestic_Total_Gross, Distributor, Release_Date,Runtime	Production_Budget, MPAA_Rating, and Genre


### 2.2 Data Cleaning and Feature Engineering

The next focus was to clean the data to build a better model. I started by importing the CSV file that I had created into my Python environment then I read this file using dataframes.Next, I worked with the variables to make sure that they were able to be processed by applied the following: 

* Turning the Release Date strings into datetime objects
* Turning the runtime string from "1 hr. 52 min." to minutes float format
* Getting the Month , Day of Year and Day form Release Date
* Dealing with categorical data such as Genre and MAPP Rating
* Drop the Null values
* Shuffling Data

Regarding dealing with categorical data I used One-Hot encoding with Genre feature and Ordinal with MAPP Rating feature

### 2.3 Model Building 

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


