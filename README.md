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

Findings
------
####Age
The first interesting point came from the data on age of all the individuals coming to the parole bard. 

####Race and Crime


Further Questions
------
####Proportions per crime and race

####Correlations and Regressions
