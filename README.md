# bike-routes
Bike route data on OpenStreetMap for LA County is sporadic and seems to be based on varying standards. Import current County and City datasets and update existing information.

## Class Tags
* ICN: based on the [OSM guidance](http://wiki.openstreetmap.org/wiki/Cycle_routes) there are currently no ICN entries in the LA area
* NCN: USBR 66 would be national. It is still only proposed, but seems to already be tagged on OSM. Should this be retagged?
* RCN: does California have any recognized regional routes?
* LCN: the named bike paths listed [on Wikipedia](https://en.wikipedia.org/wiki/List_of_Los_Angeles_bike_paths), ensuring that the names used match the signage (for example, the new Expo line path is signed as "Expo Bike Path" rather than "Expo Bikeway")
* Unnamed routes (typically Class II / III)

Need to somehow separate Class I (actual bike paths) from Class II (painted lane on side of the road) and Class III (sharrows and/or occasional signs next to the road, i.e. largely meaningless).

## Links
Some links with further information:
* http://egis3.lacounty.gov/dataportal/2013/05/29/bike-paths/
* http://developer.metro.net/introduction/bikeways-data/download-bikeways-data/
* http://dpw.lacounty.gov/bike/map.cfm
* http://wiki.openstreetmap.org/wiki/California/Cycling_Relations
* http://wiki.openstreetmap.org/wiki/Cycle_routes
* http://wiki.openstreetmap.org/wiki/United_States/Bicycle_Networks
* https://data.lacounty.gov/Shape-Files/LA-County-Bikeways/brdh-e23g
* https://data.lacity.org/A-Livable-and-Sustainable-City/Bikelanes/uzvv-a9xz
* http://geohub.lacity.org/datasets/230abc621b144dbc96cca83d65bd454d_0
* https://en.wikipedia.org/wiki/List_of_Los_Angeles_bike_paths
* http://bike.lacity.org/
