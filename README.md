# Big_Data_Data_Ingestion_-_Processing
Use Hive to analyse the trips made New York Taxi and Limousine Commission

Problem Statement
The New York City Taxi & Limousine Commission (TLC) has provided a data of trips made by the taxis in the New York city. The detailed trip-level data is more than just a vast list of taxi pickup and drop off coordinates. 

The records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations (location coordinates of the starting and ending points), trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts etc

By aggregating the aforementioned records this dataset was created that provides precise location coordinates for where the trip started and ended, timestamps for when the trip started and ended, plus a few other variables including fare amount, payment method, and distance travelled.

In this assignment, we ONLY consider the data of yellow taxis for November and December of the year 2017.

 

Download the dataset from the following links and push it into your S3 bucket.

NYC Yellow Taxi's trip data for November 2017

NYC Yellow Taxi's trip data for December 2017

 

 

The problem statement is mentioned below.

 

Basic Data Quality Checks

How many records has each TPEP provider provided? Write a query that summarises the number of records of each provider.
The data provided is for months November and December only. Check whether the data is consistent, and if not, identify the data quality issues. Mention all data quality issues in comments.
You might have encountered unusual or erroneous rows in the dataset. Can you conclude which vendor is doing a bad job in providing the records?
 

Analysis-I

Compare the average fare for November and December.
Explore the ‘number of passengers per trip’ - how many trips are made by each level of ‘Passenger_count’? Do most people travel solo or with other people?
Which is the most preferred mode of payment?
What is the average tip paid? Compare the average tip with the 25th, 50th and 75th percentiles and comment whether the ‘average tip’ is a representative statistic (of the central tendency) of ‘tip amount paid’.
Explore the ‘Extra’ (charge) variable - what is the fraction of total trips where an extra charge is levied?

Analysis-II

What is the correlation between the number of passengers and tip paid? Do multiple travellers pay more compared to solo travellers?
Create five buckets of ‘tip paid’: [0-5), [5-10), [10-15) , [15-20) and >=20. Calculate the percentage share of each bucket (i.e. the fraction of trips falling in each bucket).
Which month has a greater average ‘speed’ - November or December? Note that the variable ‘speed’ will have to be derived from other metrics.
Analyse the average speed of the most happening days of the year i.e. 31st December (New year’s eve) and 25th December (Christmas Eve) and compare it with the overall average.
