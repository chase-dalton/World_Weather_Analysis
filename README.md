# World_Weather_Analysis

## Overview
The purpose of this analysis was to retrieve weather data from the OpenWeatherMap API, create a customer travel destinations map based off of user input using Google Maps, and create a travel itinerary map in Google Maps using the Google Maps Directions API.

## Process
Using Python, a list of random latitudes and longitudes was generated. Using Citipy, the nearest city for each lat and long combination was found to generate a list of cities. Then using the OpenWeatherMap API, weather data such as temperature, wind speed, and weather description was pulled in to create a Weather CSV to be utilized for the Customer Travel Destinations Map.

![weatherdb](https://github.com/typicalchazz/World_Weather_Analysis/blob/main/Weather_Database/Weather_DB.png)


Once the Weather CSV was created, it was utilized in a DataFrame by the Customer Travel Destinations Map. Users are prompted to choose a temperature range for their desired trip and that input would filter the Weather DataFrame and by using the Google Maps API, hotel JSON data was appended to city and weather information to return a DataFrame of cities in a certain temperature range that included hotel options. Using Google Maps, the hotel data was added to a map layer to return a map with city markers with hotel and weather information included.

![search](https://github.com/typicalchazz/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)


Finally, using the previously mentioned map and DataFrame, as well as Google Directions API, a travel itinerary was created where a travel map was generated between 4 selected cities to show the ideal route between them.

![itinerary](https://github.com/typicalchazz/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
