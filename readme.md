FGx Globe
===========

[ FGx copyright notice and license](https://github.com/fgx/fgx.github.com/blob/master/FGx%20copyright%20notice%20and%20license.md)

2013-02-25 ~ just getting off the ground...

Geographic data represented on spheres has certainly created some pretty maps.

But can a globe be used to represented non-geographical big-data in successful ways?

This repository is about the exploration of such possibilities.

The first data globe to arrive here is FGX Globe.

FGX Globe acquires data from [FGX](http://www.fgx.ch/). FGX builds add-ons for [FlightGear](http://www.flightgear.org/) - the popular FOSS flight simulator, 

In particular, FGX Globe uses the [Crossfeed](http://crossfeed.fgx.ch/data) near real-time data feed which shows all the Internet-connected planes in the air.

For the latest updates please have a look at [FGx Open Source Projects](http://fgx.github.com)


## Change log

/2013-05-03 ~ Theo
* smaller file size models from FG via blender
* fgx globe: seymour is pre-loaded

2013-05-02 ~ Theo
* fgx globe airports: lot of UI work

2013-05-01 ~ Theo
* Loaded Aerostar model - exported from FlightGear

2013-04-30 ~ Theo
* Load multiple types of planes
* Eight types of models now avalable
* Improved call back handling
* Improved already loaded handling
* More logical variable names
* Better deletion of terminated flights
* Aircraft scale changes with camera distance
* Camera motion stops when you zoom in

2013-04-28 ~ Theo
* Number of planes shows in window title bars
* Planes are now all b777 3D models
* Flight windows with OSM has select zoom and retained in permalinks
* Flight windows now show a 2D image of plane rotated to current headding 
* The main menu is using small text in most places
* Text on Info page updated

2013-04-27 ~ Theo
* 4flight-window-settings.html: simplified JavaScript and HTML
* 3globa-settings.html: simplified JavaScript and HTML
* 0info.html tidied
* Added more maps
* Planes are deleted as and when Crossfeed no longer lists them
* Windows stay closed - and are deleted from the permalink 
* started work on bringing in 3D models

2013-04-26 ~ 
* Updated index page for fgx-globe
* Added load-plane-3d
* Updated fgx-globe-r3

2013-04-19 ~ Theo
* Added j3QUE FGx r1
* New index page for fgx-globe
* fgx-globe-r2-dev uses updated Crossfeed link 

2013-04-13 ~ Theo
* World Airports,Runways and Navaids r2.4: airport image links to Google Maps
* World Airports,Runways and Navaids r2.4: tightened up Heads-up diaply
* World Airports,Runways and Navaids r2.4: added link to wunderground.com

2013-03-20 ~ Theo
* airport symbol size is scaled to the camera distance
* display output prettified with degree symbols
* Checked Geoff's naivaid file for commas in name field. Found none
* Deleted quotes from file. Reduced file size by 3%
* Checked Geoff's icao file for commas in name field. Found none
* Deleted quotes from file. Reduced file size by 4.2%
* Replaced custon XMLHttpRequest functions with generic function
* Was loading two starfield bitmaps, now just one!

2013-03-19 ~ Theo
* updates to airports-runways-navaids r2.2
* Added loading, reading display of Geoff's navaid data
* Completed namespacification
* Added mousewheel event capture and linked it to onMouseUp function

2013-03-18 ~ Theo
* update airports-runways-navaids r2.1
* Distance calculations now relate to camera position, not a separate airplane object
* Number of airports displayed relates to camera altitude versus number of ILS and distance from camera
* Scale of airport symbols relates to alitude
* Settings display updated
* Heads-up display shows number of runways and ILS
* More variables embedded in the FGx name space  
* Ongoing code clean-up

2013-03-17 ~ Theo
* Added airports-runways-navaids r2
* r2: skysphere with one of Paul Blunt's PNGs
* r2: globe has texture
* r2: added lights
* r2: fixes silly bug where heads-up displayed incorrectly. Fixed position of sidebatr causing issue

2013-03-09 ~ Theo
* Adding airports-runways-navaids folders + data

2013-03-09 ~ Theo
* Adding copyright and licensing information

2013-03-07 ~ Theo
* added word-wrap:break-word; to heads-up css in globe-circumscribe-airports-2k-json.html

2013-03-06 ~ Theo
* added aptinfo folder with navaid data for 2,123 airports
* cookbook: added globe-circumscribe-airports-2k-json.html 
- not fully working

2013-03-05 ~ Theo
* cookbook: added open-geoff-file-head-ups-only-nearby.html
- Shows details of nearest of 27,000 airports
* cookbook: added globe-circumscribe-airports.html
- ditto with nicer UI
* cookbook: added globe-circumscribe-airports-2k-only
- what does a globe with 2,134 airports look like? Crowded.


2013-03-04 ~ Theo
* cookbook: added 'open-geoff-file-show-only-nearby.html'

2013-03-03 ~ Theo
* cookbook: added 'open-geoff-file-and-display.html'
* cookbook: added 'open-geoff-file-and-find-nearby.html'

2013-03-02 ~ Theo
* cookbook: added 'find-nearby.html'
* cookbook: added 'globe-circumscribe.html'

2013-03-02 ~ Theo
* Wiki: worked on mission statement 

2013-02-28 ~ Theo
* Started & completed process of putting variables in a name space. Thanks to Pete for the push...
* mothball: looks for latest update number otherwise delete...
* Added GoSFO and GoWorld ~ wormholes into parallel worlds

2013-02-27 ~ Theo
* Updated public home page regarding dev version, new code 
* default camera position is set by laitude, longitude and radius using new update position function
* Started adding API with access via query string 

*2013-02-26 ~ Theo
* Rejigged placard and heads-up distrubition of info
* Added display of thumbnails to heads-up where model thumbnails exist.

2013-02-25 ~ R2 ~ Theo  
* Started Change Log in GitHub Read Me  
* Created folders for textures & fgx-globe r2 & populated fgx-globe-r2  
* OBJ.planeId.hdg & dist_nm: no longer arrays, now single values  
* Addeded OBJ.planeId.update  
* Moved propellers back into correct location r1 + r2  
* Cleaned up processFlightsData()  
* Added 'mothball' function - to remove non-active planes from the scene  
* Updated text to show the count of 'flying' and 'flown'  
* Added an Equator  
* Added back skywriting  

2013-02-25 ~ R1 ~ Theo  
* simplified object management
* globe has diameter of 100 units
* planes have heading - but I think they are off by 90 degrees or 270 or something but I have not taken the time to track this down yet.
* sliders allow you to set plane scale and altitude scale
* planes with an altitude of 0, are grayed.
* moving the cursor over a plane cause a 'heads-up' display to appear which displays model name and the remaining data from the feed not shown on the placard

