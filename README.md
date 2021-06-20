# Python API Challenge
## Python API Homework - What's the Weather Like?

---
### Task
In this task we have been asked to answer the question "What's the weather like as we approach the equator?"

The first part of the task is *Part 1: WeatherPy*. The details for this section are below.
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

The second part of this task is *Part 2: VacationPy*. The details for this section are below.

Based on the cities.csv file created in part 1, we need to create a heatmap that displays each cities humidity.
Next we narrow down the list of cities based on some weather parameters to find our ideal weather selection.
A Google Places API is then used to find the first hotel for each city located within 5000 meters of the cities coordinates.
The hotels are then plotted ontop of the heatmap and a pin is displays the Hotel Name, City and Country.


---
### Method

Part 1: WeatherPy

The code begins by generating a random list of cities from the citipy Python library. This code was prewritten and we simply required to run it.
Note: I have inserted np.random.seed(11) at the top of the code so that I could get the same list of cities each time and not have to change my analysis results when completing the graphs. To get a new list of cities, simply remove the random.seed line. Please also note that this could result in cities with a greater humidity than 100 - these cities need to be dropped by there is no code to complete this step since it was not required for my cities list.

Once the cities list is generated we are going to use the weather maps API and compile the weather data for each of the cities found. 
For this section we start by establishing the url required to make the API call.
We then create empty lists that will be filled by a for loop that goes through each city in the list and gets the data we have defined.

The lists are populated with the below data:

* The city name
* The max temperature
* The humidity
* The cloudiness
* The wind speed
* The cities Country
* The date
* The latitude
* The longitude




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
