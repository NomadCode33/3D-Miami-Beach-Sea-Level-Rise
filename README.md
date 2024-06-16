# City of Miami Beach Sea Level Rise
A dynamic 3D map highlighting the buildings in Miami, Florida that are projected to be at risk from rising sea levels by 2050.

**Link to project:** http://recruiters-love-seeing-live-demos.com/

![alt tag](http://placecorgi.com/1200/650)

## How It's Made:

**Tech used:** ArcGIS Pro, ArcGIS Online, ArcGIS Living Atlas of the World, ArcGIS 3D Analyst extension

I first downloaded the dataset of Miami. Then I had to transform the 2D map into a 3D map display and later set the extrusion of the buildings. After the extrusion, I joined the tables to transfer attributes for the exact accurate building heights using the join field tool since beforehand every building was the same size even though in real life every building varies in size and structure. To make the buildings more aligned with real life, multipatch layers were created. By using the symbology pane and the rule package file (RPK), instead of flat surface designs for the buildings it shoewed more detailed textures and windows. Not only that but installing the RPK file changed the roof shape of the buildings. I then added in the data for water and make it into a realistic 3D representation of how it looks like in real life through the symbology pane. After that I set the illumination setting to set the display 3D scene reflect the lighting at certain times of day. The time I set was 8AM.



Went onto ArcGIS Living Atlas of the World to get layers of intermediate-high sea level rise of the years in 2030, 2050, and 2090 from NOAA's Digital Coast

Used the Environments Geoprocessing tool to configure sea level data.
Then used a raster to polygon tool to convert raster data to polyogn in order to be used. Now the sea level rise data is more interactable in polygon form than in raster form for future analysis

I then calculated the affected buildings by filtering the building layer with the 2030, 2050, and 2090 intermediate-high sea level rise data using the Select by Location tool
- When i opened the attribute table, it showed he selection of the buildings affected by said year.
- Within the attrivute table I created a new column called Inundated year to show which buildings are at risk for that repsective year
- I repeated the process for 2050 and 2090

Using the Symbology pane, I then created unique values that properly showed which building is affected by a certain year and changing the color scheme to reflect that. green meaning not affected, 2030 being light-orange, 2050 being dark orange, and 2090 being red

I used the Elevation Profile tool to measure elevation in buildings. Turns out that buildings that aren't affected are built at higher elevation and were built with sea level rise in mind. The buildings at risk of being destroyed weren't built with that in mind. This makes it so that buildings in development are built with sea level in mind.

Lastly, I uploaded the 3D map onto ArcGIS Online.


Here's where you can go to town on how you actually built this thing. Write as much as you can here, it's totally fine if it's not too much just make sure you write *something*. If you don't have too much experience on your resume working on the front end that's totally fine. This is where you can really show off your passion and make up for that ten fold.

## Optimizations
*(optional)*

You don't have to include this section but interviewers *love* that you can not only deliver a final product that looks great but also functions efficiently. Did you write something then refactor it later and the result was 5x faster than the original implementation? Did you cache your assets? Things that you write in this section are **GREAT** to bring up in interviews and you can use this section as reference when studying for technical interviews!

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable
