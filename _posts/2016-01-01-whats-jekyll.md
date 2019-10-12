---
layout: post
title: Project3 :Direct Marketing Campaign
date:               2019-10-12 23:22:00 +0000
---



## 1. Objectives



In fact, marketing spending in the banking industry is massive, meaning that it is essential for banks to optimize marketing strategies and improve effectiveness. In this project, I try to answer the question, how to increase the effectiveness of the bank's telemarketing campaign? The major goal is to predict a customers' response to the telemarketing campaign and establish a target customer profile for future marketing plans.In sum, the classification model used to predict if the client will subscribe to a term deposit or not.




## 2. Workflow
The following figure shows the workflow of Predicting Movie Domestic Total Gross 
![Image test]({{ site.url }}/images/project3-1.png)



### 2.1 Description of Dataset

In this project I obtained the dataset from  from [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/datasets/Bank+Marketing#)


![Image test]({{ site.url }}/images/project3-2.png)



### 2.2 Data Cleaning 

The next focus was to clean the data to build a better model. I started by importing the CSV file that I had created into my Python environment then I read this file using dataframes.Next, I worked with the variables to make sure that they were able to be processed by applied the following: 

* Checking Null Values
* Deleting unnecessary features such as duration of call
* Dealing with Unknown Categorical Values by predicting the unknown values using cross-tabulation
* Dealing with Categorical Values ( One Hot Encoding and Ordinal Converting)
* Scaling the data


### 2.3 Exploring Bank Marketing Dataset 
After data cleaning steps completed,then I start to exploring bank marketing dataset. Generally, before starting building the model we should check many things. First, I create an initial plot of target value to look to the distribution. From the following figure, the initial plot looks like unbalance data likes most of the marketing dataset.

The following figures describe the dataset of bank marketing 

#### 2.3.1 Pre-Model Building 

After data cleaning steps completed,then I start to building the linear regression models.Generally, before starting building the model we should check many things. First, I create an initial plot of Domestic_Total_Gross to look to the distribution. From the following figere the initial plot looks like normal distribution so there is no need to do the log transformation

![Image test]({{ site.url }}/images/project3-3.png)


![Image test]({{ site.url }}/images/project3-4.png)



![Image test]({{ site.url }}/images/project3-5.png)


![Image test]({{ site.url }}/images/project3-6.png)

#### 2.3.2 Model Building

![Image test]({{ site.url }}/images/project3-7.png)


## 3. Results

![Image test]({{ site.url }}/images/project3-8.png)


## 4. Resource Description
For more details please viste [Project Resource](https://github.com/LubnaAlhenaki/sa19_ds1/tree/master/student_work/project2/Lubna_Alhenaki). This repo contains the following:
* Movie2018 that contain the code file.
* Project-02 pdf file that describe the project in details.

Also I recommended [The determinants of box office performance in the film industry revisited](https://pdfs.semanticscholar.org/c960/7aaa7746ec9735a19d0ab2e524e53d20ab7f.pdf) scientific paper


