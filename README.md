# Mapping-with-D3---590v-HW3
Files for 590v HW3 -  mapping with D3
590v HW3 : Mapping with D3

Question 1:
The dataset used pertains to known meteorite sightings all over the world. The dataset is created and maintainted by NASA and is available for download from the nasa.gov or data.gov APIs. It contains information about over 45000 known meteorite sightings. The dataset is around 5 MB in .csv format. The dataset was converted into geoJSON format for use with our map and comes to around 18 MB in this format. It contains the name, mass, location, type and other information about the meteorites. It can be used to get an insight about the geo-spatial distribution and density of the meteorites across the world. The meteorites are also classified by the type of sighting i.e., whether a meteorite 'fell' or was 'found'.

Question 2:
The projection we use here is the very popular Mercator projection. We use this as it a standard projection to use for the world map. It is a cylindrical map projection presented by the Flemish cartographer Gerardus Mercator in 1569. It became the standard map projection for nautical purposes because of its ability to represent lines of constant course, known as rhumb lines or loxodromes, as straight segments that conserve the angles with the meridians. Although the linear scale is equal in all directions around any point, thus preserving the angles and the shapes of small objects (which makes the projection conformal), the Mercator projection distorts the size of objects as the latitude increases from the Equator to the poles, where the scale becomes infinite. So, for example, landmasses such as Greenland and Antarctica appear much larger than they actually are relative to land masses near the equator, such as Central Africa. One measure of a map's accuracy is a comparison of the length of corresponding line elements on the map and globe. Therefore, by construction, the Mercator projection is perfectly accurate, k = 1, along the equator and nowhere else. This is actually true of many projections in that they are not perfectly accurate as the spherical shape of the earth cannot be directly translated onto a 2D plane (paper/screen), hence the need for various projections. However, for our purposes, the Mercator projection suffices.

Question 3:
The map is drawn using world.json and uses Mercator projection. The points are plotted using meteorites.geojson and each point represents a sighted meteorite. 

Question 4:
Here, we allow the user to hover over each of the points to display the name and mass information of each meteorite on the side.

Question 5:
We provide a slider to select the type of sighting, which as previously mentioned can take values 'Fell' or 'Found'. The map is refreshed and points highlighted according the slider selection.

Question 6:
We build the svg container element in a way as to allow for zooming in and out. The initial state looks as though it's zoomed in a little. It actually displays the map area with the most concentrated meteorite density. The map can be zoomed out to show the full projection and can be panned or zoomed in to take a closer look at a desired region.
