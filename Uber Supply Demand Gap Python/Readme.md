## Problem Statement
### Introduction

This data set is a masked data set which is similar to what data analysts at Uber handle. Solving this assignment will give you an idea about how problems are systematically solved using EDA and data visualization. 

## Business Understanding

You may have some experience of traveling to and from the airport. Have you ever used Uber or any other cab service for this travel? Did you at any time face the problem of cancellation by the driver or non-availability of cars?

Well, if these are the problems faced by customers, these very issues also impact the business of Uber. If drivers cancel the request of riders or if cars are unavailable, Uber loses out on its revenue. You can learn more about such problems that Uber faces during its operations in the video linked below. You will be hearing from Sai Alluri he was a data analyst at Uber and has worked on this problem. 

## Uber business problem explanation

As an analyst, you decide to address the problem Uber is facing - driver cancellation and non-availability of cars leading to loss of potential revenue.

## Data Understanding

Download the dataset from [here](https://cdn.upgrad.com/UpGrad/temp/76b3b6a4-d87d-4e82-b1c3-3f6e10b9c076/Uber%20Request%20Data.csv)

There are six attributes associated with each request made by a customer:

    Request id: A unique identifier of the request
    Time of request: The date and time at which the customer made the trip request
    Drop-off time: The drop-off date and time, in case the trip was completed 
    Pick-up point: The point from which the request was made
    Driver id: The unique identification number of the driver
    Status of the request: The final status of the trip, can be either completed, canceled by the driver or no cars are available

** Note: For this assignment, only the trips to and from the airport are being considered.**

 

## Data Cleaning and Preparation - Hints

    Identify the data quality issues and clean the data so that you can use it for analysis.
    Ensure that the dates and times are in the proper format. Derive new variables which will be useful for analysis.

 
## Results Expected

    Visually identify the most pressing problems for Uber. 
        Hint: Create plots to visualize the frequency of requests that get canceled or show 'no cars available'; identify the most problematic types of requests (city to airport/airport to city etc.) and the time slots (early mornings, late evenings etc.) using plots
    Find out the gap between supply and demand and show the same using plots.
        Find the time slots when the highest gap exists
        Find the types of requests (city-airport or airport-city) for which the gap is the most severe in the identified time slots
    What do you think is the reason for this issue for the supply-demand gap? Write the answer in less than 100 words. You may accompany the write-up with plot(s).
     Recommend some ways to resolve the supply-demand gap.

 

Present the problem, the analyses and the recommendations using plots to the Chief Data Scientist in a well-formatted presentation (make sure to submit a PDF version of the PPT). Also, include a commented jupyter Notebook in your submission. Please note that the assignment has to be done completely in Python including the plots. However, you may recreate the plots in Tableau to include in the presentation.