EDA_Project_2021_NYC_subway

NYC Guide Dogs - Fund Raising Support

Abstract

The goal of this project was to recommend to a fiction charity the best times and locations to their fund raising stations. The New York City Guide Dogs Foundation has limited budget available for ad, so they set up some criteria what the project had to follow.
The New York City subway's turnstile data was the source of my project which is available on the MTA's website [MTA data](http://web.mta.info/developers/turnstile.html). From the downloaded data the analysis represents the time periods of the stations with the highest number of entries. In the visualization of the results I used bar and line charts to represent the busy stations on the investigated period and for each months/weeks.

Design

The NYC Guide Dogs Foundation supports blind and vision impaired people living in New York City. Their job is huge help for these people but the activity they do very expensive and they have limited budget for running fund raising events. The previous years experience was that the charity received the most donations around Christmas time.
The Foundation required the analysis to meet with the following criteria: 
1) the locations should be selected from the NYC subway stations, 
2) the project should recommend no more than 5 weeks of period between November and January. 
In line with their requirements we aimed to recommend 5 times 1 busy week on different subway stations.
With our help the charity will be able to get in touch with many people and provide information of their activities and mission for a wide audience.

Data

The MTA's website includes the turnstile data files what I used to the analysis. These reports has records of the entering and exiting traffic of each individual turnstiles in every subway stations in New York City. The audit of the data occurs every 4 hours of the day. The original data included the cumulative data incoming and outgoing traffic.
The data of the project represents the period between November 2020 to January 2021.

Algorithms

A few issues were found in the original data. Some typo corrections and cleaning tasks needed to process initially to be able to get insight information in the data during the analysis. The cumulative data of the entering traffic caused another problem to the further work on the data which was fixed by calculating the daily entries of each turnstiles. 

After the data preparation we identified the 10 Stations with the highest entering traffic.
As the first 5 stations are not in the same neighborhood we processed further analysis on the monthly and then weekly data of these stations. As an additional information we provided the busiest day of the week to each stations (according to average entries number of each station in the selected period).

Our recommendation for the client is the following:

1) 34 St - Herald Square - 3rd week of November -  Tuesday
2) Grand Central - 42 St - 3rd week of November - Monday
3) Flushing - Main - 3rd week of November - Tuesday
4) 42 ST-PORT AUTH - 4th week of January - Tuesday
5) Path New WTC - 2nd week of January - Wednesday


Tools

1) Data Collection - SQL system  
2) Data Preparation:  - Python via SQLAlchemy
3) Exploratory Data Analysis - Python Pandas package
4) Data Visualization - Python Matplotlib package


Communication

The results of the project represented on line and bar charts. 
![Top_10_stations](https://raw.githubusercontent.com/NemeGabi/Metis-EDA-Project/master/Top_10_stations_data.png)

![Top_5_stations](https://raw.githubusercontent.com/NemeGabi/Metis-EDA-Project/master/Top_5_weekly_traffic.png)

![Top_5_stations_dayofweeks](https://raw.githubusercontent.com/NemeGabi/Metis-EDA-Project/master/Top_5_per_daysofweeks.png)

