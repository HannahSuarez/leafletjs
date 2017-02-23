<a href="http://hannahsuarez.me/projects/MapboxJS/mapbox-noir.html" target="_blank"><img src="http://hannahsuarez.me/projects/MapboxJS/mapboxanim.gif"></a>

<a href="http://hannahsuarez.me/projects/MapboxJS/mapbox-noir.html" target="_blank">View the full map</a>

#OpenStreetMap and LeafletJS example 
In this example, I am using LeafletJS which is an open source mapping library for building interactive maps. You can use this LeafletJS with Mapbox or another map platform. In this example, I am using OpenStreetMap.

Locate the html file containing the initial code in the Github repository.

##Adding your own map

To add your map, go to http://openstreetmap.org and search for the location where you want to add the marker. After searching for the location you will notice that the URL will change. Use the values in this URL to add the longitude, latitude and zoom values within the map variable:
````
var map = L.map('map',{scrollWheelZoom:false}).setView([longitudeValue, latitudeValue], zoomValue);
```
To add a custom marker, replace the iconURL and iconSize with your own.

To add the location of your custom marker, you can use http://openstreetmap.org to give you an idea of what the longitude and latitude values are and replace below:
````
var marker = L.marker([longitudeValue, latitudeValue], {icon: customIcon}).addTo(map);
````
There is a lot more that you can do with LeafletJS http://leafletjs.com/index.html
