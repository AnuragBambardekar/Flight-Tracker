# Real-Time Flight Tracker
This Python script uses the Bokeh library to create a real-time flight tracker. It fetches live flight data within a specified geographical area and plots the aircraft positions on a map.

## Dependencies
OpenSky API
Bokeh
Numpy
Requests
Pandas

## How it works
- The script first defines the geographical boundaries for the flight tracker.
- It then sends a request to the OpenSky Network’s API to fetch live flight data within these boundaries.
- The flight data is stored in a pandas DataFrame.
- The script converts the geographical coordinates (latitude and longitude) to Web Mercator coordinates, which are used by the Bokeh library for plotting.
- The Bokeh figure is set up with the specified x and y ranges.
- The flight data is plotted on the map using the image_url and circle methods from Bokeh. The image_url method is used to plot an icon for each aircraft, and the circle method is used to plot a circle marker for each aircraft.
- A hover tool is added to the plot, which displays information about the aircraft (call sign, origin country, velocity, and altitude) when the user hovers over an aircraft marker.
- Labels are added to the aircraft markers, displaying the call sign of each aircraft.
- Finally, the plot is displayed using Bokeh’s show method.

## Future Work
- Live Flight Tracking

## References:
- https://openskynetwork.github.io/opensky-api/rest.html - OpenSky API <br>
- https://www.geodose.com/2020/08/create-flight-tracking-apps-using-python-open-data.html - Flight Tracker tutorial <br>
