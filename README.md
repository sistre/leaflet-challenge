# leaflet-challenge
Leaflet Homework - Visualizing Data with Leaflet

This repository contains two levels of vizualizing earthquake data from the USGS "Past 7 Days" "All Earthquakes" GeoJSON located at:
https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson

## Level 1: Basic Visualization
This vizualization plots the earthquake locations with both size and color based on the magnitude on a light grayscale map of the world. When an earthquake is clicked on, a popup is presented showing the earthquake's magnitude, location, and date/time. There is also a legend displayed that shows the magnitude to color association.

A live version can be seen here: https://sistre.github.io/leaflet-challenge/Leaflet-Step-1/index.html

## Level 2: More Data
The second vizualization builds on the first by adding base map choices (Satellite, Grayscale, and Outdoors) and a plot of the Earth's tectonic plate fault lines. The ability to toggle the fault lines and earthquakes has also been added. The fault line data is being pulled directly from the "raw" data in the PB2002_boundaries.json file located in the GeoJSON folder at https://github.com/fraxen/tectonicplates.

A live version can be seen here: https://sistre.github.io/leaflet-challenge/Leaflet-Step-2/index.html

## How to test the files in this repository
The files in this repository can be run as-is when downloaded and placed in the same file scructure. However, both levels require an additional file named config.js to be place in the /static/js folder. This file requires the following line of code which requires a token from Mapbox.com:

const API_KEY = "<Place Mapbox Token Here>";

