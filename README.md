# World_Weather_Analysis

## Overview of Project
Make improvements to the PlanMyTrip app using API calls of Open Weather, Google Places, and Google Directions API. The PlanMyTrip app helps users find hotels in locations all around the world based on temperature preference. From there, the user will be able to see the city, temperature, humidity, cloudiness, and weather description of the hotel locations. Finally, the app will select 4 nearby hotels and plan a "fake" trip for the user.

## Resources
Software: Python 3.7.13, Jupyter Notebook 6.4.8, Anaconda 4.13.0, Visual Studio Code 1.68.1  
API's Used: [OpenWeather](https://openweathermap.org/), [Google Places](https://developers.google.com/maps/documentation/places/web-service/search-nearby), 
and [Google Directions](https://developers.google.com/maps/documentation/directions/overview)

## Results
### Weather Database
After getting 2,000 random latitudes and longitudes worldwide and finding the nearest city, I would up with 783 random cities. Using the OpenWeather that is linked above, the weather at these given cities was parsed through and gathered in the [WeatherPy Database](/Weather_Database/WeatherPy_Database.csv). This captures the City, Country, Latitude, Longitude, Max Temperature, Humidity, Cloudiness, Wind Speed, and Current Weather Description for July 21st, 2022 at 783 random cities.

### Vacation Search
Once the weather data has been populated, we can ask the user for information! The program allows the user to select the minimum and maximum temperature they would like their vaction to be and we can filter based on that information. Then, using Google Places API we find the nearest hotel to each location that fits the user's criteria. For example, the below diagram show what having a temp range between 75°F and 90°F:

[](/Vacation_Search/WeatherPy_vacation_map.PNG)

We see the app is able to return the Hotel Name, City, Country, and Current Weather of all the locations that fit the users temperature preferences.

### Vacation Itinerary
And lastly the app can also plot a example roadtrip getaway. Using four cities near each other in the Northeast part of the United States, we can create a route and display the same markers as above:

[](/Vacation_Itinerary/WeatherPy_travel_map.PNG)
[](/Vacation_Itinerary/WeatherPy_travel_map_markers.PNG)

These improvements will help users find hotels that suit their weather preferences and plan a getaway vacation!