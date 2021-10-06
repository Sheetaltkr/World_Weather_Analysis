# World Weather Analysis

## Overview

Plan My Trip is a top Travel Technology company which provides online services in Hotel and Lodging industry.

The purpose is to:

-	Help Jack (head of analysis for the User Interface team of PlanMyTrip App) collect and present data to find the best cities for a vacation based on certain weather criteria and then map these cities using **Jupiter G maps** and the **Google places API**. This will help "Plan My Trip" enhance their customer search on their PlanMyTrip app.

- Create a travel route between the four potential travel destination cities as well as a marker layer map using the **Google Maps Directions API**.

### The analysis of the data is divided into three main stages
1.	Collect the Data
2.	Exploratory Analysis with Visualization
3.	Visualize Travel Data


### Collect the Data:  Weather Database

The **`Weather_Database.ipynb`** program uses **Open Weather Map API** to pull weather information on over 690 various cities around the world and save city weather data in **`WeatherPy_Database.csv`** file. The weather metrics gathered are:

1. Maximum Temperature
2. Cloudiness
3. Wind Speed
4. Humidity
5. Current Weather Description

This city weather data forms the super-set for the specific weather search criteria used in the next exploratory analysis stage.

### Exploratory Analysis with Visualization: Vacation Search

The **`Vacation_Search.ipynb`** program uses the city weather data from **`WeatherPy_Database.csv`** and **Google Maps API** to create a subset data of cities complying to selected weather criteria and saves it in **`WeatherPy_vacation.csv`** file. The data is then used to plot these travel destinations with a hotel at each city location on Google map. The map below shows the cities with hotels that have an daily maximum temperature between **75** and **90** degrees Fahrenheit. 

![vacation_search_map](https://github.com/Sheetaltkr/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)	

### Visualize Travel Data: Vacation Itinerary

This **`Vacation_Itinerary.ipynb`** program uses the subset data from **`WeatherPy_vacation.csv`**, and **Google Maps directions API** to create a vacation itinerary. The **WeatherPy_travel_map** below shows a 4 stop itinerary in USA  that features **Buckeye, San Patricio, Spring Hill and Elizabeth city** with Buckeye as  as the start and end point of the travel itinerary.

![vacation_itinerary_map](https://github.com/Sheetaltkr/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

- **WeatherPy_travel_map_markers** Map below shows the hotels at the cities and its current weather

![vacation_itinerary_markers](https://github.com/Sheetaltkr/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
