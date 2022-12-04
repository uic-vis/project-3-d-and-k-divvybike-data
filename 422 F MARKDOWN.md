422 FINAL PROJECT MARKDOWN DOCUMENT - BY KESHAV AND DAKSHYA

LINK TO THE WEBSITE - https://sites.google.com/uic.edu/422project3


For this final project we chose Chicago Taxi Trips dataset. This dataset has all the information of the taxi trips that took place in the month of February and June. Our data set contains 23 coloums. 

1) Trip ID - A unique identifier for the trip.
2) Taxi ID - A unique identifier for the taxi.
3) Trip Start Timestamp - When the trip started, rounded to the nearest 15 minutes.
4) Trip End Timestamp - When the trip ended, rounded to the nearest 15 minutes.
5) Trip Seconds - Time of the trip in seconds.
6) Trip Miles - Distance of the trip in miles.
7) Pickup Census Tract - The Census Tract where the trip began. For privacy, this Census Tract is not shown for some trips. This column often will be blank for locations outside Chicago.
8) Drop Off Census Tract - The Census Tract where the trip ended. For privacy, this Census Tract is not shown for some trips. This column often will be blank for locations outside Chicago.
9) Pickup Community - The Community Area where the trip began. This column will be blank for locations outside Chicago
10) Drop Off Community - The Community Area where the trip ended. This column will be blank for locations outside Chicago.
11) Fare - The fare for the trip.
12) Tips - The tip for the trip. Cash tips generally will not be recorded.
13) Tolls - The tolls for the trip.
14) Extras - Extra charges for the trip.
15) Trip Total - Total cost of the trip, the total of the previous columns.
16) Payment Type - Type of payment for the trip.
17) Company - Name of the Taxi Company 
18) Pickup centroid Latitude - The latitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.
19) Pickup Centroid Longitude - The longitude of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.
20) Pickup centroid location - The location of the center of the pickup census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.
21) Dropoff centroid latitude - The latitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.
22) Dropoff centroid longitude - The longitude of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.
23) Dropoff centroid Location - The location of the center of the dropoff census tract or the community area if the census tract has been hidden for privacy. This column often will be blank for locations outside Chicago.


Data Visualization 1 - Ride distribution 

![Screenshot%202022-12-04%20at%202.47.13%20PM.png](attachment:Screenshot%202022-12-04%20at%202.47.13%20PM.png)

For this we found the distribution of the number of rides between all the cab companies and what the most popular areas for that particular cab company are. 

We used the total number of the rows with each company name, and displayed it. As for the map, we used the ['Pickup Centroid Longitude'] and ['Pickup Centroid Latitude'] to map the x and y location of each pickup location. For bar chart, we used only the 'Company' attribute.

The interactive part of this is that the map shows the pick up locations of the taxi company we select from the chart above. Depending on the taxi company we select the density of the pick up locations change as every taxi comapany's rides differ





Data Visualization 2 - Total Income 

![Screenshot%202022-12-04%20at%202.47.33%20PM.png](attachment:Screenshot%202022-12-04%20at%202.47.33%20PM.png)

For this visualization we found out the total income of all the cab companies in a normal month and a holiday season month to see if there is a increase in the income amount. Apart from this we found the difference amount between the income for both the months. 

Top three taxi company's income during normal season in the month of February  :

1)Flash Cabs - $160000

2)Taxi Affiliation LLC - $130000

3)Sun Taxi - $65000


Top three taxi company's income during holiday season in the month of June :

1)Flash Cabs - $270000 - Still the most dominant

2)Taxi Affiliation LLC - $250000 - Almost doubled

3)Sun Taxi - $150000 - More than doubled


Even though the top three companies remain the same for the both seasons the income of the other Taxi companies has significantly 
increased during holiday season compared to the normal season.

For this chart, we used the ['Trip Total'] and ['Company'] attribute, where we summed the trip total for each company and added it into an object. For the whole dataset, we extracted the month number of each row. Then when dropdown value is changed, we filtered the dataset based on the selected month from the dropdown then updated the bar chart based on the filtered data.

For the interactive part, we included a dropdown menu to choose the month. In this that is February or June. The chart will update and show the total income for a taxi company for that specific month. 

Data Visualization 3 - Payment type

![Screenshot%202022-12-04%20at%202.47.54%20PM.png](attachment:Screenshot%202022-12-04%20at%202.47.54%20PM.png)



With this chart we found the common modes of payment for Chicago taxi customers. This pie chart shows the data for six specific days. Three in the month of February which is a normal month and three days in the month of June as it is a holiday month. 

Which ever day you pick the most common use of payment method is credit card followed by cash followed by mobile payment.

For the interactive part the user can hover over any part of the pie chart to see what the percentage of that payment method is. 

we used  the '['Payment Type']' for pie chart. For percentage, we divided the total number of each 'payment type' by the total dataset length. For the slider, we first converted the format into 'dd-mm-yyyy' format, then added each unique date into an array, then created the slider based on those unique dates. Then when the value of slider is changed, we filtered the dataset to return only the rows where date=selected slider date and then updated the pie chart based on the filtered data.







Data Visualization 4 - Popular pick up points - New Spatial view.

![Screenshot%202022-12-04%20at%203.20.48%20PM.png](attachment:Screenshot%202022-12-04%20at%203.20.48%20PM.png)

Finally now that we found out the popular taxi companies and their total income. We wanted to find the popular locations for picking up passengers in the city of Chicago. This chart does exactly that by showing the number of rides in that particular area. 

For the interactive part the user can hover over any hotspots on the map to know the exact number of pickups that took place in that area in that particular month. The only problem we faced with this chart is that the pick up locations especially in the downtown area were very close to each other resulting in congested dots on the map. 






