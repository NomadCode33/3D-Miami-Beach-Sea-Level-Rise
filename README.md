# City of Miami Beach Sea Level Rise
A dynamic 3D map highlighting the buildings in Miami, Florida that are projected to be at risk from rising sea levels by 2050.

**Link to project:** http://recruiters-love-seeing-live-demos.com/

![alt tag](http://placecorgi.com/1200/650)

## How It's Made:

**Tech used:** ArcGIS Pro, ArcGIS Online, ArcGIS Living Atlas of the World, ArcGIS 3D Analyst extension

I began by downloading the dataset of Miami and transforming the 2D map into a 3D display. The next step was to set the extrusion of the buildings. After the extrusion, I used the join field tool to merge tables, transferring attributes to accurately reflect the varied building heights, as initially, all buildings were the same size. To further align the buildings with their real-life counterparts, I created multipatch layers. Utilizing the symbology pane and a rule package file (RPK), I enhanced the buildings with detailed textures and windows, and the RPK file also modified the roof shapes for realism. I then added water data, creating a realistic 3D representation through the symbology pane, and set the illumination to reflect 8 AM lighting conditions.

With the basics completed, I focused on acquiring sea level rise data from the ArcGIS Living Atlas of the World, specifically layers for intermediate-high sea level rise projections for 2030, 2050, and 2090 from NOAA's Digital Coast. I used the Environments Geoprocessing tool to configure this data, and the raster to polygon tool to convert the data into polygons for better interactivity. 

Next, I calculated the affected buildings by filtering the building layer using the Select by Location tool with the sea level rise data for 2030, 2050, and 2090. In the attribute table, I created a new column called "Inundated_Year" to indicate the year each building is at risk. Using the symbology pane, I assigned unique colors to reflect the risk levels: green for not affected, light-orange for 2030, dark-orange for 2050, and red for 2090. 

To further analyze, I used the Elevation Profile tool to measure the elevation of buildings, finding that those not at risk were built at higher elevations with sea level rise in mind, unlike the vulnerable buildings. This insight emphasizes the importance of considering sea level rise in future building developments.

Finally, I uploaded the 3D map onto ArcGIS Online for public viewing.

## Optimizations
*(optional)*

You don't have to include this section but interviewers *love* that you can not only deliver a final product that looks great but also functions efficiently. Did you write something then refactor it later and the result was 5x faster than the original implementation? Did you cache your assets? Things that you write in this section are **GREAT** to bring up in interviews and you can use this section as reference when studying for technical interviews!

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable
