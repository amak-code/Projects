# Covid_Map Project

This project is a Covid Data Map visualizing Countries Covid Data on a Global Map ( last update from 12/25/2021).
It is made on Jupyter Notebook using Pandas and Folium Libraries.

DATA:
The Covid data was taken from "JHU CSSE COVID-19 Data" (url: https://github.com/CSSEGISandData/COVID-19)
I also use another csv file with the Population Data from kaggle.com (https://www.kaggle.com/tanuprabhu/population-by-country-2020).
I joined two DataFrames together, removed some columns and created two new columns("Mortality" and "Main_data")
The final DataFrame consists of 7 columns and I changed the index from numbers to Country names.

CONTENT:
The data contains the following information:
-Lat;
-Long;
-Confirmed Covid cases;
-Deaths;
-Population(2020);
-Mortality per 100,000 population(("Deaths" * 100000)/"Population(2020)")
-Main Data(Country Name + Confirmed cases + Deaths + Mortality)

VISUALIZATION:
Using Folium Library I created Interactive Global Map with icons for every contry. 
It shows the Country name if you hover over the icon.
If you click on icon it shows: Country Name + Confirmed cases + Deaths + Mortality per 100,000 population ()
The data from "Main Data" column is used for popup.
The data from "Lat" and "Long" columns used for country location on the Map.

https://amak-code.github.io/Projects/Covid_map/map.html
