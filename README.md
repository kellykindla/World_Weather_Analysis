# World_Weather_Analysis 
# Module6

## Project Overview
### Purpose of Module 5 
For this module, we were challenged to expand our knowledge of python libraries and modules in efforts to perform analyses and visualizations on data retrieved from APIs. The API data were stored as JSON arrays and was analyzed through scatterplots and Google Maps heatmaps. 

### Overview of Assignment 
For this module and challenge, we utilized “get” requests to collect random latitude and longitude coordinates from the CityPy module and the OpenWeatherMap API. From these coordinates, we collected weather data from cities around the world to analyze with Matplotlib library’s scatterplots and Google Maps API’s. We initially plotted the relation between latitude and weather conditions (temperature, humidity, cloudiness, and speed) and created linear regressions for each condition for both the Northern and Southern Hemispheres to determine if the was a correlation between the condition and latitude. We further translated the weather data into a series of heatmaps using Google Maps and Places API. 
The series of heat maps and their associated scatter plots are shown below:

Latitude vs Temperature:

<img width="870" alt="TempHeatMap" src="https://user-images.githubusercontent.com/92558842/143975605-ad9cc513-3719-46d5-adb2-149c9ad24c73.png">
<img width="476" alt="MaxTempVLatNorth" src="https://user-images.githubusercontent.com/92558842/143975616-53cddb6a-3e40-4ff0-aa5d-0e3b4ec4456c.png">

Latitude vs Humidity:

<img width="867" alt="HumidHeatMap" src="https://user-images.githubusercontent.com/92558842/143975703-9add4a1a-4ae0-40b0-9fa5-a2c85ce57441.png">
<img width="465" alt="HumidVLatNorth" src="https://user-images.githubusercontent.com/92558842/143975630-5fcc7e02-df57-446d-806e-a5989ae57cff.png">


Latitude vs Cloudiness:

<img width="869" alt="CloudHeatMap" src="https://user-images.githubusercontent.com/92558842/143975720-a35ef8a1-b96c-4317-a864-bc012fb15fc3.png">
<img width="466" alt="CloudVLatNorth" src="https://user-images.githubusercontent.com/92558842/143975760-cdd793f1-0190-41df-8a86-c9498ac63fb5.png">


Latitude vs Wind Speed:

<img width="867" alt="WindHeatMap" src="https://user-images.githubusercontent.com/92558842/143975728-e1695d40-b71e-45a2-b011-3384d6f89043.png">
<img width="453" alt="WindVLatNorth" src="https://user-images.githubusercontent.com/92558842/143975773-f3f9fe10-d02b-4b1c-b1dd-a8ffbabf8050.png">

For the challenge, we altered our DataFrame to include the weather description. A sample of the DataFrame is shown below. 

<img width="793" alt="Challenge_city_data_df" src="https://user-images.githubusercontent.com/92558842/143976017-d282bc59-6338-4694-8d73-3eb2926913e6.png">


To make our analysis interactive, we used input statements to retrieve customer weather preferences to identify potential travel destinations and nearby hotels based on their ideal temperature range. A new DataFrame was created based on the user selection and was displayed with a marker map and is displayed below for an example range of 60 to 80 degrees Fahrenheit. 

<img width="881" alt="WeatherPy_vacation_map" src="https://user-images.githubusercontent.com/92558842/143976072-574e1ac7-a68d-48bd-b1cf-b37b5a9e4288.png">

Lastly, based on the user’s weather preferences, we used Google Directions API to create a travel itinerary showing the route between four cities. For my analysis, displayed below, the four Australian cities were: Yulara, Broken Hill, Port Augusta, and Esperance. After discovering the latitude- longitude pairs for each city, we created a directions layer map where the start and end point were Yulara. This direction layer map is shown below: 
<img width="871" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/92558842/143976130-c9c26d06-7400-47cd-b184-8b0e754a82fe.png">

To further display the customer’s itinerary, we combined the weather data for the four cities into one DataFrame and refactored our code to display the marker layer map shown below: 
<img width="870" alt="WeatherPy_travel_map_markers" src="https://user-images.githubusercontent.com/92558842/143976142-41a77b9e-6f64-49b1-8874-1ac0aeb7a524.png">


### Resources
The data for Module 6 were taken from the OpenWeatherMap API and Google Maps API
#### Software used:
	- Python 3.7.10
	- Anoconda 4.10.1
	- Jupyter Notebook 6.3.0
	- Matplotlib 3.3.4
