# Academic Projects
Projects done in ArcGIS Pro during my BS program at the University of Kansas.

## How Consistent is Kansas Precipitation? 

<img width="2000" height="1294" alt="image" src="https://github.com/user-attachments/assets/1190146f-37cc-4f7a-a6c7-bc755e10c469" />

This project was for a cartography class where I got to experiment with different design techniques. 

The precipitation data is from the Kansas Office of the State Climatologist (K State Weather Data Library). This provided annual precipitation data for Kansas counties from 2014 - 2024. I pulled all the data into one Excel file, calculated the mean and standard deviation of rainfall per county, and then derived the coefficient of variation (CV) from it.  <br>
<p align="center">
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/b346ab11-86a6-47c8-80e0-4680061d013a" />
 </p>
I used an SQL query to only label cities with a population greater than 126,000 and I removed the city of “Overland Park” because it was competing for space between the “Kansas City” and “Olathe” label. After this, western Kansas had almost no city labels, so I added “Hays” and “Dodge City” because those are two cities that are decently populated. Later in the design process, I added “Liberal” in Seward County because I made a callout for Seward (as the county with the most variation), and I thought it would be helpful to show a populated city there. 
 
## Temporal Expansion of Antarctic Research Infrastructure
<img width="2000" height="1294" alt="image" src="https://github.com/greenchristina/Academic-Projects/blob/ead9124eee73e5a5323e6148327a7974d4b4e7c8/Screenshot%202026-02-18%20192613.png" />
For this project, my goal was to create a map that shows the historical development of Antarctic research stations across five major eras: the Heroic Age (1895 - 1922), the Mechanical Age (1923 - 1946), the Pre-IGY Cold War Expansion (1947 - 1956), the Post-IGY Cold War Expansion (1957 - 1991), and the Modern Scientific Era (1992 - present). I wanted to highlight how, even though Antarctica is often seen as remote and unchanging, the establishment of research stations over time reflects major scientific, political, and technological shifts. By combining temporal classification with geographic visualization, I was able to show both the chronology and the spatial distribution of Antarctic scientific activity.<br>

<br>For my data, I used the COMNAP Antarctic Facilities CSV file, which includes the location, operational status, station name, and establishment year for all permanent year-round research stations. After downloading the CSV, I used the XY Table to Point tool in ArcGIS Pro to convert the latitude and longitude fields into a point feature class. Once I created the points, I used the Define Projection tool to assign the correct coordinate system. I also used a shapefile of the Antarctic continent from the British Antarctic Survey, which includes continent boundaries and ice shelf outlines. To add some texture to the map, I found a DEM of Antarctica on ArcGIS Online and exaggerated the z-value in ArcGIS Pro so the elevation data would enhance the map without distracting from the main theme.
