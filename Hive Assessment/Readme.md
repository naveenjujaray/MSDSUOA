Problem Statement
Objective

The assignment is meant for you to apply the learnings of the module on Hive to a real-life dataset. One of the major objectives of this assignment is to gain familiarity with performing analytics with Hive.

 
Problem Statement

New York City is a thriving metropolis, and like most other cities of its size, one of the biggest problems faced by its residents is the lack of parking space. The classic combination of a huge number of cars and cramped geography is the exact recipe that leads to a large number of parking tickets.

 

In an attempt to scientifically analyze this phenomenon, the NYC Police Department regularly collects data related to parking tickets. This data is made available by the NYC Open Data portal. Your job is to try and perform some analysis on this data in order to answer the questions that follow.

 

Note: The data for 2017 has been uploaded on an S3 bucket at the following link:

s3://hiveassignmentdatabde/Parking_Violations_Issued_-_Fiscal_Year_2017.csv

 

STEPS BELOW FOR SETTING UP:

    You have been given this data set in the S3 bucket. For the command mentioned below, you need to download this data into the EMR cluster from the given public S3 bucket. You need to follow the given steps you have followed in the last sessions:

    wget  https://hive-assignment-bucket.s3.amazonaws.com/Parking_Violations_Issued_-_Fiscal_Year_2017.csv;

     
    In case S3 bucket is down, please find the alternative steps mentioned at the bottom of this page.

    Launch Hive and create a database. 

    Create tables inside the database as per the CSV file; delimited by ‘|’ and lines separated by ‘\n’.

    Next, you have to move the tables you downloaded from S3 by using the command

        load data <local path of S3 file> into table <table name> ;

         

 

Consider only the data for the year 2017 itself for your analysis, not the current year.

 

The data dictionary is available on this page.


The analysis can be divided into two parts:

 
Part-I: Examine the data

    Find the total number of tickets for the year.
    Find out the total number of states to which the cars with tickets belong. The count of states is mandatory here; providing the exact list of states is optional.
    Some parking tickets don’t have addresses on them, which is a cause for concern. Find out the number of such tickets which have no addresses. (i.e. tickets where one of the Street Codes, i.e. "Street Code 1" or "Street Code 2" or "Street Code 3" is empty)

 
Part-II: Aggregation tasks

    Find out the frequency of parking violations across different times of the day: The Violation Time field is specified in a strange format. Find a way to make this into a time attribute that you can use to divide into groups.
    Divide 24 hours into six equal discrete bins of time. The intervals you choose are at your discretion. For each of these groups, find the 3 most commonly occurring violations.
    Now, try another direction. For the 3 most commonly occurring violation codes, find the most common times of day (in terms of the bins from the previous part).
    Let’s try and find some seasonality in this data:
        First, divide the year into seasons, and find the frequencies of tickets for each season. (Hint: A quick Google search reveals the following seasons in NYC: Spring(March, April, May); Summer(June, July, August); Fall(September, October, November); Winter(December, January, February))
        Then, find the 3 most common violations for each of these seasons.

 

To analyze the date-time variables, you could use inbuilt Hive functions. Please find reference documentation along with examples on the below-mentioned links:

1. Apache Hive documentation

2. Hive tutorial for date-time format

 

Note: Please ensure you make necessary optimizations to your queries, like selecting the appropriate table format and using partitioned/bucketed tables. 

 

Dataset mirror links: 

In case the HTTP S3 link seems to be down. The data can be copied to personal S3 by using the following command:

#Working with EMR Cluster
aws s3 cp s3://hiveassignmentdatabde/Parking_Violations_Issued_-_Fiscal_Year_2017.csv s3://<bucket-name>

Or you can download the CSV file from this link.

 
All The Best!!!