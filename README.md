# Carbon Offset Project Locations

Most Verra and CAR projects include a geospatial file. This can be accessed from the registry websites. Additionally, Verra includes the location in the JSON file that feeds the project description sites.

I downloaded the geospatial files (shapefile or KML) when available, and computed the lat,lon of the centroid of the shapes in the file.

Sometimes, Verra's location from the JSON is nonsense, so the geospatial files are useful in that case. Also, these are more accurate (assuming shapefile is correct).

This method can be used to access the location of all CAR and Verra projects automatically should you ever need it.

Files:

* Folder [locationFiles](locationFiles) includes the location files downloaded from the registries
* [Voluntary registry database](Voluntary-Registry-Offsets-Database--v8-May-2023.xlsx) is the Berkely's database I used to retrieve data in a cleaner way
* [getProjects](getProjects.ipynb) is the script to download the files from the registries
* [readLocation](readLocation.ipynb) is the script to read the lat,lon from the files
* [mapPlot](mapPlot.ipynb) is a simple interactive map showing the projects
* [projectsManual](projectsManual.csv) is the final version of the data with the manual adjustments I did for some projcts.
