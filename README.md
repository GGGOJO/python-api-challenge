# python-api-challenge
This challenge was to send a request to two APIs and extract data to analyze weather and geolocation data. I used OpenWeatherMap API and Google Places API for the two parts of this challenge.

## Part I - WeatherPy
Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. Using various Python packages and a little common sense to create a representative (Regression) model of weather across world cities.

Start an extraction:

    Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude from citipy.
    Perform a weather check on each of the cities using a series of successive API calls.
    Include a print log of each city as it’s being processed with the city number and city name.
    Save a CSV of all retrieved data and a PNG image for each scatter plot.
 
Once the data has been extracted, clean, and saved into a new df and exported into a .csv file, the coding, visualizations, and analysis may begin!

The first set of visualizations is a series of scatter plots to showcase the following relationships. After each plot, add a sentence or two explaining what the code is analyzing.

    Temperature (F) vs. Latitude
    Humidity (%) vs. Latitude 
    Cloudiness (%) vs. Latitude
    Wind Speed (mph) vs. Latitude

The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

    Northern Hemisphere - Temperature (F) vs. Latitude
    Southern Hemisphere - Temperature (F) vs. Latitude
    Northern Hemisphere - Humidity (%) vs. Latitude
    Southern Hemisphere - Humidity (%) vs. Latitude
    Northern Hemisphere - Cloudiness (%) vs. Latitude
    Southern Hemisphere - Cloudiness (%) vs. Latitude
    Northern Hemisphere - Wind Speed (mph) vs. Latitude
    Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, a few thoughts were provided to explain what the linear regression is modeling. For example, describe any relationships that I noticed or recommendations for further analysis if given more time or data.

## Part II - VacationPy
Planning for future vacations when we are able to travel freely without COVID-19 restrictions! Using jupyter-gmaps and the Google Places API for this part. I had to use !pip jupyter nbextension enable --py gmaps in my environment.

First step is to read the .csv dataset of cities from Part I.

Next is to create a heat map that displays the humidity for every city from Part I. 

Then, filter out cities that meet the following "ideal weather" criteria:
  A max temp < 80 degrees
  A max temp > 90 degrees
  Wind speed < 10 mph
  Cloudiness == 0 
  Drop any rows that do not meet these conditions.

Use Google Places API to find the first hotel for each filtered city that is located within 5,000 meters of my city's coordinates.

Plot the hotels on top of the first heat map that pins the Hotel Name, City, and Country.

##Written Oberservations
For Part I, 
  3 overall written observations of the WeatherPy have been placed at the top of the notebook. 
  1-2 sentences were provided for each plot within the WeatherPy notebook
 
For Part II, 
  Two screenshots were provided - the original heatmap and the marked layer heatmap.

##Reflections/After Thoughts
The most difficult part of this challenge was getting the Google api key. I started early to register for one but when I tried to used it in Jupyter Notebook, I received error messages. I'd like to use Google maps again for other analysis coding, but it seems the biggest hurdle is getting the api key to work?!?


