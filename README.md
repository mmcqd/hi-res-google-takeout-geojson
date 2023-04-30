# hi-res-google-takeout-geojson

Inspired by: https://community.esri.com/t5/arcgis-data-interoperability-blog/get-your-google-location-history-on-the-map/ba-p/1154723

This script uses the Google Routes API to create high resolution geojson data describing your movements as tracked by Google.

At https://takeout.google.com/ you can download all the location tracking data Google has on you. 

It contains a bunch of json files in a custom format. If you convert them directly to geojson, you'll get a bunch of ugly, spiky lines.

We can improve this by using the Google Routes API to ask for the best route between each recorded location. You'll have to include your own API key in the script.

You can paste the resulting geojson data into geojson.io to visualize it.
