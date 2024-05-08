# IGTProject
Plotting the location of every library in our state (Maharashtra) and create an interactive map/web map

Project Topic:

Find the location of every library in your state and create an interactive map/web map.

Abstract:

The project aims to address the challenge of locating libraries across Maharashtra by creating an interactive web map. Leveraging data from government sources and mapping technologies, the project aims to provide a user-friendly platform for accessing information about libraries in the state. By converting raw data to CSV format, utilizing OpenStreetMap (OSM) for mapping, and integrating user-friendly features, the project endeavours to enhance access to library services for students, researchers, and the public.

Methodology:

We have imported the base layer OSM standard (OpenStreetMap) using QuickMapServices plugin in QGIS. We imported the state boundaries of India as a shapefile and formatted the appearance to highlight our zone of emphasis. Using QuickOSM plugin, we ran a query to locate all libraries in Maharashtra in the OSM database and added those as points. This layer was saved in the project file. We collected data about the libraries in Maharashtra and their addresses from the Directorate of Libraries, Government of Maharashtra Higher and Technical Education Department https://dol.maharashtra.gov.in/en/govt._recognized_public_libraries. We found the coordinates of these libraries using mapping services like Google Maps and added those to a csv file, which was later imported as a delimited text layer after appropriate coordinate system conversion (Google Maps Global Mercerator EPSG:4326 WGS84 to OSM WGS84 Pseudo Mercerator EPSG:3857). Using Google MyMaps, we created a map and searched for all libraries in Maharashtra and imported the map as a kmz file (view the map here). After tweaking the aesthetics, we exported the project as a webmap using the qgis2web plugin. The exported project was uploaded on Netlify and deployed (https://librariesmaharashtra.netlify.app/).

![image](https://github.com/tana13p/IGTProject/assets/143800660/7fff8afb-211d-499c-b132-de8ecdd22965)
