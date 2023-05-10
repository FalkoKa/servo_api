# Servo API

Group project.

An app to show your current location, to find where the closest service station is based off the location you put into the map.

![Servo API screenshot](/public/icons/servoapi.png)

# Features

The app uses server requests from a database to render requests from the database about the locations of various service stations. It includes a search function to find locations on the map, information about the owners of each service station, current location displayed and service stations closest to them, spotlighted info for a random service station, dynamically displayed markers that appear as the center of the map is changed and oil prices based of current oil prices.

# Map API

The map is used to display information based off the database, the database takes the latitude and longitude and places that location into the map that dynamically places the markers on the map based off the map center.

# Database

The datatbase contains information of every service station. It is called either randomly, to fetch a random pertrol station and display that in the spotlight, all service station within the bounds of what is currently visible on the map. The owners of each petrol station and the amount of petrol stations they own and the current nearest stations to the current centre of the map within a 5km distance of the location.

# Distances

Distances are processed through postgresql query string that is then sorted via the alogithm places into it. The lognitude and latitude for the current center of the map is then found and processed through the algorithm in the postgresql query. It then shows sorts the information by those closest to the current map center before being dynamically displayed on the sidebars.

# Oil prices

Oil prices are fetched through the commodiites api, the JSON response object is then displayed on the screen.

# Languages

Javascript, CSS, HTML, EJS, NodeJS, postgreSQL, axios libraby for AJAX requests.

By

- Henry: https://github.com/henry-rennell
- Elmira: https://github.com/elmira1788
- Falko: https://github.com/FalkoKa
- Jack: https://github.com/jrh1010101101010
