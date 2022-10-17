# Ford GoBike System Data Exploration

## by Michal Chiagoziem Ezeh


## Dataset

> This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The data was obtained from the dataset options 
presented by Udacity in section 1.1. The dataset contains 183,412 records and 16 features:
start_time
end_time
start_station_id
start_station_name
start_station_latitude
start_station_longitude
end_station_id
end_station_name
end_station_latitude
end_station_longitude
bike_id
user_type
member_birth_year
member_gender
bike_share_for_all_trip.

>This is the URL in which the dataset can be gotten from:
ford_gobike_url = 'https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv'

>Before exploration, some data wrangling steps were performed were changing the datatype of some features and the are:
>- changing data type of start_time and end_time to datetime.
>- changing data type of member_birth_year to integer which was initially in float.
>- converting bike_share_for_all_trip to bool.


## Summary of Findings

> After wrangling, I set out to figuring out how the trip duration is dependent on the other features in this dataset and the following features used to show the dependency were: duration_sec, start_station_id, end_station_id, member_birth_year, user_type, start_hour,
start_day. I started my exploration using the univariate, bivariate and multivariate exploration. 

> Univariate Exploration
In this exploration which makes use of individual variables, I observed:
>- Some stations in this dataset see more activity than others.
>- Using the log-transform of the trip's duration, it gives us a distribution we can more easily understand and relate with, a right-skewed normal distribution, with most of the trips les than 2000 seconds, and the most trips taking around 400 - 700 seconds.
>- The distribution of the age of users that most users are between 20 to 45 years old.

> Bivariate Exploration
In this exploration which makes use of  relationships between two pairs of variables, I observed:
>- By using the heatmap, the users of bikes aged between 20 and 45 tend to take the longest time completing their rides.
>- The higher percentage of customers are taking longer trips then compared to subscribers.
>- A bimodal distribution of rides during weekdays with peak periods at 8AM and 5PM. However, on weekends, peak period is around 1-2PM, and it is not bimodal.

> Multivariate Exploration
In this exploration which makes use of  relationships between three pairs of variables, I observed:
>- From the multivariate analysis of start day, start hour and duration_sec, we observe that the longest trips tend to start in the early hours of the morning, typically before 6AM.
>- Customers tend to have the longest trip durations, with a peak at 3AM in the morning. On the other hand, the average ride duration for subscribers is quite low when compared to that of the customers, and is quite similar across the hours of the day.



## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.
From the Ford GoBike dataset exploration, I was able to observe the relationship of different features and I answered my question of how the time duration is dependent on variables such as user type, birth year and the time and day etc.







