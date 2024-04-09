<h1 align="center">DU - DA Module 15 "leaflet-challenge"<br/>
An Interactive Earthquake Map</h1>
<h2 align="center">Using HTML(PyCharm), CSS, JavaScript(Visual Studio Code), and the D3 and Leaflet libraries<br/>
<br/>
by Laura Vara</h2><br/>

![ForReadMe_mapWTEXT](https://github.com/vara-co/leaflet_challenge/assets/152572519/2f8cc091-0bc3-4867-b28d-09b6db44e5f2)


**Live Interactive Leaflet-Challenge HTML Deployment website:** https://vara-co.github.io/leaflet_challenge/

The goal of this assignment was to build an interactive Earthquake visualization with information from the [USGS GeoJSON Feed](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) website.
Note that I used the 'Feed', which is the column on the right side, for the 'Past 7 Days' for All Earthquakes. This can be updated in the code with a different link to see different date parameters or be selective with different magnitudes.

<h2>Index</h2><br/>
1. Content of the repository<br/>
2. Instructions for the Challenge<br/>
3. References<br/>

Content of the repository
-----------------------------------------------------------
- index.html    <-- This is the HTML used to deploy the map in a website
- static directory:
  - CSS directory:
    - style.css    <-- css file that will need to be updated to display the legend on the map
  - js directory:
    - logic.js   <-- file that contains the code to make the map interactive and display the data collected.
- Leaflet-Part-1 directory: <-- this directory is just to comply with the instructions of this assignment. It's the same files as above.
  
(Note that for the paths that connect the HTML with the style.css file and the logic.js file, the order in which they are in, has to be in the same order they have been uploaded in this repository. Othewise you would have to redefine the file paths in your HTML code.)

<h2>Instructions</h2>
The instructions for this challenge are divided into the following subsections:

<h2>Part 1: Create the Earthquake Visualization</h2>
 
![image](https://github.com/vara-co/leaflet_challenge/assets/152572519/7adc1087-0830-4e77-9c28-11151dfa3b81)

<h3>1. Get your dataset. To do so, follow these steps:</h3>

- The USGS provides earthquake data in a number of different formats, updated every 5 minutes. Visit the [USGS GeoJSON Feed](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) page and choose a dataset to visualize. The following image is an example screenshot of what appears when you visit the link:

![image](https://github.com/vara-co/leaflet_challenge/assets/152572519/d6012dfe-a4b0-4b26-b9e9-1571a4da861a)
  
- When you click a dataset (such as "All Earthquakes from the Past 7 Days"), you will be given a JSON representation of the data. Use the URL of this JSON to pull in the data for the visualization. The following image is a sampling of earthquake data in JSON format:

![image](https://github.com/vara-co/leaflet_challenge/assets/152572519/48d58547-5967-4566-a1e5-16c087fd4165)

<h3>2. Import and visualize the data by doing the following:</h3>

- Using leaflet, create a map that plots all the earthquakes from your dataset based on their longitude and latitude.
  - Your data markers should reflect the magnitude of the earthquake by their size and the depth of the earthquake by color. Earthquakes with higher magnitude should appear larger, and earthquakes with greater depth should appear darker in color.
  - **Hint:** The depth of the earth can be found as the third coordinate for each earthquake.
  
- Include popups that provide additional information about the earthquake when its associated marker is clicked.
- Create a legend that will provide context for your map data.
- Your visualization should look something like the preceding map.

<br/>

<h2>Part 2: Gather and Plot More Data</h2>
(Optional with no extra points. Note that if you don't see a Leaflet-Part-2 directory, then this section has not been made as it is optional. The information here is for references only, so I can later on work on it as practice.)

- Plot a second dataset on your map to illustrate the relationship between tectonic plates and seismic activity.
- You will need to pull in this dataset and visualize it alognisde your original data.
- Data on tectonic plates can be found at: https://github.com/fraxen/tectonicplates
- This part is completely optional; you can complete this part as a way to challenge yourself and boost your new skills.
- This bonus section should look like this:

<br/>

![image](https://github.com/vara-co/leaflet_challenge/assets/152572519/13912fed-007e-4697-a2db-2d4c4a97505f)


- Perform the following tasks for Part 2:
  - Plot the tectonic plates dataset on the map in addition to the earthquakes.
  - Add other base maps to choose from.
  - Put each dataset into separate overlays that can be turned on and off independently.
  - Add layer controls to your map
 

<h2>References for the leaflet-challenge</h2><br/>
Most of what's in this challenge, was covered in class.<br/>
The few things that either weren't or we had to reference to, are described
with it's source right below.<br/>


- Legend creation:
  - https://medium.com/@bikramkawan/css-alternating-colors-using-nth-child-for-three-elements-scss-370d636d4f40
  - https://www.w3schools.com/cssref/sel_nth-of-type.php
  - https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-last-child
  - https://developer.mozilla.org/en-US/docs/Web/CSS/grid-template-columns
  - https://stackoverflow.com/questions/35778338/custom-legend-with-r-leaflet
  - https://www.igismap.com/legend-in-leafletjs-map-with-topojson/#google_vignette
  - https://blog.rtwilson.com/automatically-generating-a-legend-for-a-choropleth-layer-in-leaflet/
  - https://www.amcharts.com/docs/v4/concepts/legend/
  - https://tilemill-project.github.io/tilemill/docs/guides/advanced-legends/
  - https://stackoverflow.com/questions/65042654/how-to-add-categorical-legend-to-python-folium-map

    
----------------------------------------------------------------------------------------------
