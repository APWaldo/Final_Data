Final Project for Data II
==========

Introduction
-------
This project looks at the New York State Parole Board Interview Data for 2012-2013 combined with the conviction data for each of the inmates. It tries to analyze whether there could be a connection between the given variables with the parole board information and the parole board decisions. This is a work in progress as the data set is quite complex. 


Process
------

####Cleaning
First as the data was rather unruly, it was necessary to to clean the data up to a usable format. I needed to take out all the redundant rows of information once the two data sets of parole board and conviction data were merged. Then I had to rename a lot of the variables to a more usable and understandable format. 

####Initial Analysis
With initial analysis, it was necessary to look at a summary of each variable. In order to do this, I had to convert each one to a factor. Once this was done, I realized that I had another issue: duplicated data. Because this data set contained all the interview dates of the past two years, some people were on the list multiple times, so it was necessary for me to go through the data and look for the most recent interview date and take out the rest.

Additionally, with the variable fields with dates, I had to go through and make sure that they were in R format. I alos realized that the birthdate column made it difficult to see what the true age of the person was, so I created a new column to look solely at the age of the inmate at the  time of the parole board interview. 

Also, I was able to look at crime and race up against each other, comparing the two in a mosaic plot. And then after I completed several comparisons, I was able to look at and compare race and crime and who was getting parole. Very interesting data.

Findings
------
####Age
The first interesting point came from the data on age of all the individuals coming to the parole board. The data appears to be bo or tri-modal, peaking around middle age (47-53). This could be a group of people with 20-25 years to LIFE sentences who are all hitting the parole baord at the same time. This could also be related to the kind of sentencing 20-25 years ago. This is worth exploring and looking more into.

####Race and Crime
What was so interesting about my initial mosaic plots was that most white people are going to the parole board for burglary in the second degree, whereas most black people are going to the parole board for robbery in the second degree. The difference between the two crimes is generally whether force was applied. Robbery means literal taking, whereas burglary generally means the victim is not around for the theft (houses, stores, etc.). 

Also when looking at the data for who was getting parole and who wasn't, it appears that in all cases but murder, white people are getting out on parole more than any other race. Looking at who is not getting out on parole, the majority of the inmates are black, and then other races. But this led me to a large analytical problem and error--I need to know exactly what proportion they are of the total population so I can compare like numbers (see further questions). 

Further Questions
------
####Proportions per crime and race
I need to look at proportions, not total numbers. This will give a more accurate picture of which race is getting parole per crime the most, or if they are all equal per crime (which is our null hypothesis). For this I need to create several new data sets looking at each crime and then looking closely at the racial proportion per crime. 

####Correlations and Regressions
I would like to start seeing which variables have the strongest relationships with each other. But this will only come once I create a new column for proportional population. 
