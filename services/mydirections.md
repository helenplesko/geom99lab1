# My personal directions request

First, explore the various options through the Directions API https://developers.google.com/maps/documentation/directions/get-directions. 

Be creative and use multiple parameters from the API documentation to earn a top grade. The rubric is listed in the bottom of the MarkDown document. 

> Tip: Can't make changes? GitHub previews MD documents by default (read-only). Start editing to make the changes for your URL and JSON response below

## Directions URL

Slovenia is a beautiful country and is a wonderful place to visit in the summertime. There are many sites to see there, including Ljubljana (their capital city), neighbouring towns, and century-old castles. This past summer, my family and I were able to visit the home country of my grandparents and some of the sites previously mentioned. 

Here is a driving route with an origin of Ljubljana, Slovenia, and a destination of Bled Castle, in Bled, Slovenia. From Ljubljana, the driver will stop for coffee at Slaščičarna in Kavarna Evropa in Kranj, then for gas at the OMV in Radovljica, and lastly at the Market by the Lake in Bled for a snack before heading to the Bled Castle. The route avoids tolls, the distances are in metric unit of measurement, and the departure time is set to 8am on August 1, 2024 (Slovenia time, 2am Toronto time).

```
https://maps.googleapis.com/maps/api/directions/json?origin=place_id%3AChIJ0YaYlvUxZUcRIOw_ghz4AAQ&destination=place_id%3AChIJDU8PNy2RekcRsGO3F_-nwA0&waypoints=place_id%3AChIJZTQDSR24ekcRjzqpxKImqHc%7Cplace_id%3AChIJtz8EnByWekcRaN1V-6b-Btk%7Cplace_id%3AChIJUWh1akaXekcR9HwnzRQtKBo&departure_time=1722492000&avoid=tolls&units=metric&key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE
```

I used this tool to convert the time to an integer: https://www.unixtimestamp.com/

The JSON results for this route are pasted into [mydirections.json](mydirections.json) in this repository folder.

## Optional URLs

At the second waypoint (OMV gas station) you might see some planes, helicopters, or even hot air balloons. That is because the Airport Lesce is located nearby.
```
https://maps.googleapis.com/maps/api/place/details/json?placeid=ChIJ0wL-uE-WekcR6-_C8JHoWSs&key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE
```

When at the top of Bled Castle, you get a beautiful view of the Church in the middle of Lake Bled.
```
https://maps.googleapis.com/maps/api/place/details/json?placeid=ChIJcWwyNDiRekcRQ-xUYGhbpdY&key=AIzaSyCM-WWHYHIKY-do4kquMy9Z4wQaQx51AuE
```

The URLs to view each location on Google Maps is near the end of the JSON pages above. Here they are as well for easy retrieval:

Airport Lesce:
```
https://maps.google.com/?cid=3123783530065358827
```

Assumption of Maria Church:
```
https://maps.google.com/?cid=15466868999124741187
```

I hope to go back there sometime soon!

____
## Rubric

Note: MarkDown (.md) documents are not HTML and therefore are best viewed in the github.com website, not on the pages github.io page. Marking will occur using the github.com source. 

This is part of your first practical lab in Week 3 

1. A working URL properly documented in the MarkDown and results in the JSON file with a unique origin and destination in directions earns 50%
2. Including one to four additional functioning unique parameters from the API earns 50-70%
3. Having 3 or more functioning unique/novel and well-thought out parameters from the API earns 70-90%. Explore the API documentation for parameters we have not used.
4. Tell the story of your route. Include more than 2 "stops", and/or including additional links to display PlaceIDs on Google Maps, or other innovative presentations earns 80%-100%. 
