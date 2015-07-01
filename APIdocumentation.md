# Module _pygmaps_ #

## Class _pygmaps.maps_ ##
### **Constructor _maps(latitude, longitude, zoom)_** ###
> class constructor, initialize a map  with latitude and longitude of center point and map zoom level.
  * **latitude** (float) latittude of map center point
  * **longitude** (float) latittude of map center point
  * **zoom** (int)  map zoom level 0~20
  * return the instant of pygmaps

### class maps functions ###
#### maps._setgrids(start-Lat, end-Lat, Lat-interval, start-Lng, end-Lng, Lng-interval)_ ####
  1. DESC: set grids on map
  1. PARAMETER1:	start-Lat (float), start (minimum) latittude of the grids
  1. PARAMETER2:	end-Lat (float), end (maximum) latittude of the grids
  1. PARAMETER3:	Lat-interval (float)  grid size in latitude
  1. PARAMETER4:	start-Lng (float), start (minimum) longitude of the grids
  1. PARAMETER5:	end-Lng (float), end (maximum) longitude of the grids
  1. PARAMETER6:	Lng-interval (float)  grid size in longitude
  1. RETURN:	no returns

#### maps._addpoint(latitude, longitude, `[color]`)_ ####
  1. DESC: add a point into a map and dispaly it, color is optional default is red
  1. PARAMETER1:	latitude (float) latitude of the point
  1. PARAMETER2:	longitude (float) longitude of the point
  1. PARAMETER3:	color (string) color of the point showed in map, using HTML color code. HTML COLOR CODE:  http://www.computerhope.com/htmcolor.htm e.g. red "#FF0000", Blue "#0000FF", Green "'#00FF00"
  1. RETURN:	no return

#### maps._addradpoint(latitude, longitude, radius, `[color']`)_ ####
  1. DESC: 	add a point with a radius (Meter) - Draw cycle
  1. PARAMETER1:	latitude (float) latitude of the point
  1. PARAMETER2:	longitude (float) longitude of the point
  1. PARAMETER3:	radius (float), radius  in meter
  1. PARAMETER4:	color (string) color of the point showed in map, using HTML color code HTML COLOR CODE:  http://www.computerhope.com/htmcolor.htm e.g. red "#FF0000", Blue "#0000FF", Green "#00FF00"
  1. RETURN:	no return

#### maps._addpath(path,`[color]`)_ ####
  1. DESC:		add a path into map, the data struceture of Path is a list of points
  1. PARAMETER1:	path (list of coordinates) e.g. `[(lat1,lng1),(lat2,lng2),...]`
  1. PARAMETER2:	color (string) color of the point showed in map, using HTML color code HTML COLOR CODE:  http://www.computerhope.com/htmcolor.htm e.g. red "#FF0000", Blue "#0000FF", Green "#00FF00"
  1. RETURN:	no return

#### maps.draw(file) ####
  1. DESC:		create the html map file (.html)
  1. PARAMETER1:	file (string) the map path and file
  1. RETURN:	no return, generate html file in specified directory


### class maps attributes ###