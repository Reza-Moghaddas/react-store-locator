# react-store-locator
Store locator
In this project, you will show a marker for the store that the user chooses from the dropdown!


Start by replacing the access token with your own access token. You can get it from the previous project or your mapbox account.
Create a marker that has the same position as the map's center. That's longitude, latitude: 12.567898, 55.67583. Here's how you create a marker in JavaScript:
const marker = new mapboxgl.Marker()
  .setLngLat([0, 0]) //longitude and latitude
  .addTo(map);
Handle the change event on the dropdown. We've already given you the 3 locations (longitude, latitude) for the 3 stores in the stores variable. Before proceeding to the next step, try to console.log the location of the store you select from the dropdown. Check the hints if you need help.

Change the location of the marker when the user selects a location from the dropdown. Here's how you change the location of an existing marker:

marker.setLngLat([5, 5]); //new longitude, new latitude
You will need to have access to the marker variable inside your onChange callback for it to work.

Note: in this course, mapbox is loaded in an awkward way due to a limitation with the mapbox library when running inside a browser without bundling. Inside create-react-app, you can setup mapbox by:

installing it with npm install mapbox-gl
importing it with import mapboxgl from "mapbox-gl/dist/mapbox-gl.js"
