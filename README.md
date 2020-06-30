# python-api-challenge

## Part I - WeatherPy

For this challenge, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 

To analyze the weather, I first made a series of scatter plots to showcase the following relationships:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

<img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsTemp.JPG" width="350"> <img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsHumidity.JPG" width="350">
<img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsCloudiness.JPG" width="350"> <img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsWind.JPG" width="350">


I then separated the same information into Northern Hemisphere and Southern Hemisphere and ran linear regression on each relationship.  Here is an example of the result:

<img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsTempNorthHem.JPG" width="350"> <img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/LatVsTempSouthHem.JPG" width="350">


##
### Part II - VacationPy

To plan future vacations, I used jupyter-gmaps and the Google Places API to complete the following:

* A heat map that displays the humidity for every city from the part I of the homework.

* Narrowed down the DataFrame to find my ideal weather condition:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Dropped any rows that don't contain all three conditions.

* Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

<img src="https://github.com/kelseyoros/python-api-challenge/blob/master/images/hotel_map.png" width="700">