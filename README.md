# APIs-Analysis-and-Vacation-Planner

### Tech Stack
* Python
* Jupyter Notebook
* MatPlotLib
* Pandas
* NumPy
* Google Places API
* OpenWeatherMap API 
* CitiPy 
* Jupyter-Gmaps
- - -
### User Instructions
* Clone the repository: git clone https://github.com/Vincent-glitch/APIs-Analysis-and-Vacation-Planner.git
* Open api_keys.py [API_Keys](notebooks/api_keys.py) and input your Google API key and OpenWeatherMap API key.
* Open the [WeatherPy](notebooks/WeatherPy.ipynb) file and run the cells top down.
* Open the [VacationPy](notebooks/VacationPy.ipynb) file and run the cells top down.
- - -
# Background
Analysis: This Python script uses the CitiPy library and the OpenWeatherMapAPI to visualize the weather of 500+ random cities across the world of varying distance from the equator via scatter plots. 
Planner: Using  Jupyter-Gmaps and Google Places API. This script then narrows down the locations to ones with ideal user input conditions.

## Weather Analysis

This Python script uses  the CitiPy library and the OpenWeatherMapAPI to visualize the weather of 500+ random cities across the world of varying distance from the equator via scatter plots. 

This script creates the following plots:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude
* Northern Hemisphere - Temperature (F) vs. Latitude w/ Linear Regression
* Southern Hemisphere - Temperature (F) vs. Latitude w/ Linear Regression
* Northern Hemisphere - Humidity (%) vs. Latitude w/ Linear Regression
* Southern Hemisphere - Humidity (%) vs. Latitude w/ Linear Regression
* Northern Hemisphere - Cloudiness (%) vs. Latitude w/ Linear Regression
* Southern Hemisphere - Cloudiness (%) vs. Latitude w/ Linear Regression
* Northern Hemisphere - Wind Speed (mph) vs. Latitude w/ Linear Regression
* Southern Hemisphere - Wind Speed (mph) vs. Latitude w/ Linear Regression

## Vacation Planner

Using  Jupyter-Gmaps and Google Places API this script will create a heat map that displays the humidity for every city used from the WeatherPy Analysis. This script then narrows down the locations to ones with ideal weather conditions:
* A max temperature lower than 80 degrees but higher than 66.
* Wind speed less than 5 mph.
* Less than 80% cloudiness.

This script then uses Google Places API to find the first hotel for each city located within 5000 meters of the cities coordinates and then plots the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.
