---
{"dg-publish":true,"permalink":"/campaign-1-dragoon-heist-in-krshal/player-guide/map-of-krshal/"}
---


> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`

```leaflet  
id: KrshalCityMap ### Must be unique with no spaces  
image: [[Krshal City Map Asset.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [3233, 3055]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 850px ### Size of the leaflet embed in px on your screen  
width: 95% ### Size of the leaflet embed in your note  
lat: 1616.5 ### To center the map, make this half of the map height.
long: 1527.5 ### To center the map, make this half of the map width.
minZoom: -2.3 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 0.5 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -2.3 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.75 ### Adjust how much the zoom changes when you zoom in or out.
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### marker
```
