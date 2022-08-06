### Ford GoBike System Data Analysis
The Fordgobike dataset consists of 183412 sample of different individual rides made in Ford GoBike bike-sharing system covering the greater San Francisco Bay area trips in february 2019, with 16 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip)

I cleaned missing values in start_station_id start_station_name end_station_id end_station_name, member_birth_year and member_gender features, corrected a wrong member_birth_yaer entry, converted start_time, end_time, bike_id, start_station_id, end_station_id and member_birth_year to their appropriate datatypes. I also calculated distance from start_station_latitude, start_station_longitude,end_station_latitude and end_station_longitude features and dropped them. I then converted duration_sec to duration_hr, member_birth_year to age and created age_group from age.  



## Summary of my Findings

In the exploration, I found out that majority of the riders are men from the 18-39years followed 40-60years and most of them were not just members but not subscribers. Trips occurred more from Tuesday to Friday with Thursday as the highest and Sunday the lowest while the busiest hours are 7am - 9am and 4pm - 7pm. The majority of the users are within the age of 18-39 and 40-60 which could be deduced that they are the working/business class, one could argue that the busiest hours are actually the time they should be going to work/ventures (7am - 9am) and when they should be returning home (4pm - 7pm).

 On average all age group travels almost the same distance though the tendency to travel more distance decreases as age increases. Contrary to the initial weak correlation observed between distancce_km and duration_hr, reshape  them under time series reveals that they are actually positively correlated.

Market St at 10th St generated the highest start trip while San Francisco Caltrain Station 2  generated the highest end trip. The most travelled route from our dataset is Berry St at 4th St to San Francisco Ferry Building.

The missing data we had in birth_year and gender came from stations with high demands. Thus, we can argue that the omissions might be due to rush to attend to high demands

Majority of the rides travelled alone. Customers and those with missing birth_year and gender travelled alone the most.

## Key Insights for Presentation
My presentation is based on the when( time and days ) with high rates of rides. I first looked at the riders' gender,age_group and user_type distributions. We then look at the the number of rides according to the days of the week throughout the month of febraury, the busisest time of the day uing the distance covered and finally looked at the daily distance trend.
