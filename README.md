# Bikesharing

## Overview of Analysis:
Using Tableau, create visualizations that show:

* How long bikes are checked out for all riders and genders.
* How many trips are taken by the hour for each day of the week, for all riders and genders.
* A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.

To start, I used <pandas> via <jupyter notebook> to change the tripduration column from an integer to a datetime datatype. I then saved this file as "citibike.csv" and imported the data into <Tableau>.

## Results

* First, I display the bike checkout times for each user, for every hour of a given day and the duration of that checkout. This shows the amount of bikes compared to trip times. 
  <img width="970" alt="Checkout_Times_For_users" src="https://user-images.githubusercontent.com/96043107/168639076-63417bee-7c00-477f-a336-56f2da49bd1b.png">

* Next, I display checkout-time data by gender, revealing that males have a higher checkout rate. 
  <img width="596" alt="Gender_checkout_times" src="https://user-images.githubusercontent.com/96043107/168639544-14bb263f-a845-4d9b-af00-5c121753ff32.png">

* Next, I use the "Starttime" table sorted by hour in the rows, and "Stoptime" table sorted by Weekday in the columns to display the spread of trips that occur. This heatmap shows the total count of trips for each hour on a given day.
  <img width="511" alt="Trips_weekday:hour" src="https://user-images.githubusercontent.com/96043107/168640814-7c259c5d-6374-482b-920c-4c0aad203b35.png">

* In order to further explore this data and examine trends by gender, I add a filter that allows me to sort by gender. This shows that from 7am-7pm, the male population completes the most trips out of our Female, Male, and Unknown categories. 
  <img width="1347" alt="Trips_by_gender_weekdays" src="https://user-images.githubusercontent.com/96043107/168641831-af5df65b-fbad-4e32-9f00-19b0088d994c.png">

* Furthermore, I display this gender data split into two categories (customer & subscriber) to see potential growth trends. 
  <img width="564" alt="Customer_subscriber_gender_weekday" src="https://user-images.githubusercontent.com/96043107/168641976-3b5eec7b-cf33-432a-9784-481e0477daf7.png">

## Additional Visualizations 
  
* To further explore the data, I seperated the customer vs. subscriber groups by trip duration to see the difference in trip length beteween the two segments. 

  <img width="322" alt="User_type_trip duration" src="https://user-images.githubusercontent.com/96043107/168645649-88c72463-fdde-462b-ae44-ab95e1186f6f.png">

* Lastly, I created a usertypes filter over a map that displays the counts of bicycles at end-locations, allowing me to pinpoint where majority of customers vs. subscribers end their bike rides. 
  <img width="500" alt="Usertype_subscriber_map" src="https://user-images.githubusercontent.com/96043107/168652825-0aef0a25-fe1a-4e43-b2f5-c5eb3742f093.png">
  <img width="500" alt="Usertype_customer_map" src="https://user-images.githubusercontent.com/96043107/168652865-11c1d3f4-ba79-45b1-a9a9-c09e61d59d31.png">
  
## Summary
 
My findings highlighed that for the New York Citibike program, bikes are mainly only used for about 30 minutes, with the majority of rides being about 3-8 minutes. Males use the cit bike abour 2.5 times more than females or unknown genders. On weekdays, the majority of trips are in the morning/evening hours, presumably for commuting, and on the weekends trips during the daytime are more frequent. Also, Wednesday afternoon was not a very popular time to ride for any gender. About one third of the bikes are used more fequently than the others, and the best time to service them is from about 1am-5pm. 

  
  
A link to the tableau story created for this module can be found here: [link to dashboard] https://public.tableau.com/app/profile/henry.barze/viz/Bikesharing_16527229929750/Bikesharing
