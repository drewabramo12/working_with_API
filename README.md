# working_with_API

## Overview of Project
The purpose of this project was to leverage both gmaps and OpenWeather APIs to create a desirable vacation itinerary based on temperature. The work involved the development of a random number generator for 2000 longitude and latitude coordinates. These coordinates were then used to determine nearby cities and their current weather patterns using the OpenWeather API. The gmaps API was used to depict mapping information about these locations and trip directions as well. The project was split into three stages that allowed for compartmentalizing of tasks: City aggregation, City filtering, and Directions application.

## Results

The project showed created the following maps and based on the parameters set if between 75 and 90 maximum degrees farenheit, it would be reccomended to travel to Australia for a trip.

![Temperate map](https://github.com/drewabramo12/working_with_API/blob/main/Vacation_Search/WeatherPy_vacation_map.PNG)

![Temperate map](https://github.com/drewabramo12/working_with_API/blob/main/Vacation_Itinerary/WeatherPy_travel_map.PNG)

![Temperate map](https://github.com/drewabramo12/working_with_API/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.PNG)

### Challenges
The most significant issue occurred within the creation and application of this project. The first was determining how to collect the Current Description column within the city_data DataFrame. This was solved by applying the line of code `city_current_weather = city_weather["weather"][0]["description"]`. The dictionary index indicator of `[0]` was what was missing. 

## Summary
 This script could be refactored for a multitude of weather filters and temperatures. These inputs can be used to help customers hone into exactly what time of experience they are looking for. If possible it might be worth trying to invest in getting a seven day forecast for each request to help customers think into the future on what the weather will be like for their trip.