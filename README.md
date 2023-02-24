# python-api-challenge
### Part 1: WeatherPy
In this deliverable, I create a Python script to visualize the weather of over 500 cities of varying distances from the equator. I use the citipy Python library and the OpenWeatherMap API to create a representative model of weather across cities.

##### Step 1: Creating Plots to Showcase the Relationship Between Weather Variables and Latitude

To fulfill the first step, I use the OpenWeatherMap API to retrieve weather data from the cities list. Next, I create a series of scatter plots to showcase the following relationships:
1. Latitude vs. Temperature
2. Latitude vs. Humidity
3. Latitude vs. Cloudiness
4. Latitude vs. Wind Speed

#### Step 2: Compute Linear Regression for Each Relationship

To fulfill the second step, I compute the linear regression for each relationship. The plots are seperated into the Northern Hemisphere (greater than or equal to 0 degrees latitude) and the Southern Hemisphere (less than 0 degrees latitude). 

The following plots are generated:
1. Northern Hemisphere: Temperature vs. Latitude
2. Southern Hemisphere: Temperature vs. Latitude
3. Northern Hemisphere: Humidity vs. Latitude
4. Southern Hemisphere: Humidity vs. Latitude
5. Northern Hemisphere: Cloudiness vs. Latitude
6. Southern Hemisphere: Cloudiness vs. Latitude
7. Northern Hemisphere: Wind Speed vs. Latitude
8. Southern Hemisphere: Wind Speed vs. Latitude
After each pair of plots, I explain what the linear regression is modeling as well as any relationships.

### Part 2: VacationPy

In this deliverable, the main tasks is be to use the Geoapify API and the geoViews Python library to create map visualizations.

1. A map was created that displays a point for every city in the city_data_df DataFrame. The size of the point is the humidity in each city.
2. city_data_df DataFrame was narrowed down to find the ideal weather condition. 
   Parameters:
      A max temperature lower than 25 degrees but higher than 21
      Wind speed less than 4.5 m/s
      0 cloudiness
3. A new DataFrame called hotel_df  was created to store the city, country, coordinates, and humidity.
4. For each city, the Geoapify API was used to find the first hotel located within 10,000 meters of the coordinates.
5. The hotel name and the country was added as additional information in the hover message for each city on the map
