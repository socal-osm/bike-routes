# bike-routes
Bike route data on OpenStreetMap for LA County is sporadic and seems to be based on varying standards. Import current County and City datasets and update existing information.

## Class Tags / Terminology

Relations

| OSM Relation | Description | Notes |
| --- | --- | --- | --- | --- |
| ICN | International Cycling Network | None in the LA area. |
| NCN | National Cycling Network | [USBR 66](http://www.scag.ca.gov/Documents/Bike%20Route%2066%20concept%20plan.pdf) is already tagged on OSM, but is only currently a proposed route, so this needs to be retagged as ncn=proposed. |
| RCN | Regional Cycling Network | California doesn't seem to have any recognized state routes. |
| LCN | Local [Named/Numbered] Cycling Network|The *named* bike paths listed [on Wikipedia](https://en.wikipedia.org/wiki/List_of_Los_Angeles_bike_paths), ensuring that the names used match the signage (for example, the new Expo line path is signed as "Expo Bike Path" rather than "Expo Bikeway"). Also include Bicycle Friendly Streets. |
| (none) | Unnamed Bike Routes | Any other bike routes shouldn't be marked with relations. |

Object Tags

| [OSM Tag](http://wiki.openstreetmap.org/wiki/Bicycle) | LA Metro Tag | LA City Tag | Notes |
| --- | --- | --- | --- |
| highway=cycleway | Class I | Bike Path | Separated bike path. Should normally have relation. |
| highway=cycleway | Class II | Cycletrack | [Parking-protected bike lane](http://la.streetsblog.org/2015/04/03/city-of-l-a-s-first-parking-protected-bike-lanes-reseda-boulevard/) |
| highway=\*, cycleway=lane | Class II | Bike Lane | Painted lane on side of road. |
| highway=\*, cycleway=shared_lane | Class III | Bicycle Friendly Street | [Yucca Street](https://ladotbikeblog.wordpress.com/2012/04/02/yucca-st-bicycle-friendly-street/) and Michigan Greenway in Santa Monica? Should also have relation. |
| highway=\*, cycleway=shared_lane | Class III| Sharrowed Bike Route | Sharrows on road. Typically no relation. |
| highway=\*, bicycle=designated | Class III | Bike Route | Signs alongside road. |

## Links
Data sources to investigate:
* [LA City Bikelanes, City of Los Angeles Open Data (2014-2016)](https://data.lacity.org/A-Livable-and-Sustainable-City/Bikelanes/uzvv-a9xz) and also [here](http://geohub.lacity.org/datasets/230abc621b144dbc96cca83d65bd454d_0)
* [LA County Bikeways, LA County Open Data, from LA Department of Public Works (2015-2016)](https://data.lacounty.gov/Shape-Files/LA-County-Bikeways/brdh-e23g) - includes routes in unincorporated areas plus some other major routes
* [LA County Bikeways, LA Metro (2010-2012)](http://developer.metro.net/introduction/bikeways-data/download-bikeways-data/)
* [Bicycle Routes, City of Santa Monica (2016)](https://github.com/CityofSantaMonica/GIS/tree/master/transportation/bicycle)
Information about LA region bike routes:
* [List of Los Angeles bike paths, Wikipedia](https://en.wikipedia.org/wiki/List_of_Los_Angeles_bike_paths)
* [LADOT Bike Program](http://bike.lacity.org/)
* [LA County GIS Data Portal (2013)](http://egis3.lacounty.gov/dataportal/2013/05/29/bike-paths/) - links to various data sources, all either listed above or dead links
* [Bikeways Map, LA Department of Public Works](http://dpw.lacounty.gov/bike/map.cfm) - map combining DPW and Metro (2012) data
Information about bike routes in OSM:
* http://wiki.openstreetmap.org/wiki/California/Cycling_Relations
* http://wiki.openstreetmap.org/wiki/Bicycle
* http://wiki.openstreetmap.org/wiki/Cycle_routes
* http://wiki.openstreetmap.org/wiki/United_States/Bicycle_Networks
