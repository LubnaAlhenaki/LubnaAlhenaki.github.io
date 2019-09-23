---
layout: post
title: Project3: lubna
---


<div class="message">
 Comming Soon
</div>



## 1. Objectives

WomenTechWomenYes (WTWY) is an international organizationthat aims to encourage more women to participate in the technology field. The organization hosts an annual gala at the beginning of summer in order to spread awareness towards their goal. With limited resources, they want to reach the maximum amount of people at the NYC subway stations to promote the gala and future events.



## 2. Workflow
The following figure shows the workflow of Predicting Movie Domestic Total Gross 
![Image test]({{ site.url }}/images/project2-1.png)



## 2.1 Scraping the Data
The data scraping was one of the most time consuming parts of this project because it’s difficult to navigate through the nested tables (the HTML). However, BeautifulSoup made it quite simple to grab the HTML and parse through it.

In this project I scraped from [boxofficemojo](https://www.boxofficemojo.com), I decided to start by scraping top of all  movies relased in 2018 so that I could build out my model. When I looked at the [page](https://www.boxofficemojo.com/yearly/chart/?yr=2018&p=.htm) that includes all movies that released on 2018. As a first step, I noticed that I need to collect all linkes of all movies then  go into each movie to collect the needed information. A lot of interesting information was captured in the table at the top of each movie page. The following figure is a smaple of strategy of scraping movies.

![Image test]({{ site.url }}/images/project2-2.png)
