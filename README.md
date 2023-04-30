# hi-res-google-takeout-geojson

This script uses the Google Routes API to create high resolution geojson data describing your movements as tracked by Google.

At https://takeout.google.com/ you can download all the location tracking data Google has on you. 

It contains a bunch of json files in a custom format. If you convert them directly to geojson, you'll get a bunch of ugly, spiky lines.

We can improve this by using the Google Routes API to ask for the best route between each recorded location.
