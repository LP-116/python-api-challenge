# Python API Challenge
## Python API Homework - What's the Weather Like?

---
### Task
In this task we have been asked to answer the question "What's the weather like as we approach the equator?"

Using a random list of 500+ cities we need to use an API call to determine each cities weather. This API call needs to include a print log of each city as it's being processed with the city number and city name. The results then need to be saved to a csv file.

Based on the city weather data a series of scatter plots are then generated as per below:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

We are then required to run linear regression on the below pairs:
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

An image of each plot is then saved into the out_data folder.

---
### Method


----
### Results



----
### Files

Please note you will need 2 API key's to run this code:
1. An Open weather API key (https://openweathermap.org/api)
2. A google maps API key (https://developers.google.com/maps/documentation/embed/get-api-key)
3. Create a new file in both the weatherPy and VacationPy folders to store your keys. The google maps key needs to be stored as "g_key = "ENTER CODE HERE" & the weather maps api needs to be stored under "weather_api_key = "ENTER CODE HERE". Without the API keys, the code will not run.

The WeatherPy folder also contains a folder called "output_data". Inside this folder is the cities.csv file and a saved png image of each of the plots performed in part 1.

The VacationPy folder contains a folder called "Heatmap_images". This contains a saved image of each of the heatmap images and a screen shot showing an example of how the hotel location pop up looks.
