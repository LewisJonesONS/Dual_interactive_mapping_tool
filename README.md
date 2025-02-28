# Dual_interactive_mapping_tool

A tool to map amenity locations in OS National Geographic Database (NGD) against other data sources.
In this example, the location of UK pubs is mapped from OS NGD and OS Address Base data.
The code creates an interactive map layout with two maps side by side, with synchronized zoom.
The code is generic so that datasets can be passed in to display locations of specific amenities.

## To use:

1. Create a folder with your two datasets inside it

2. Download dual_mapping_tool.ipynb to the same folder

3. Open dual_mapping_tool.ipynb in Jupyter Notebook

4. In cell 2:
    - Add the filenames for your datasets inside the brackets gpd.read_file(‘your_file.csv’)
    - Amend the titles as you wish them to appear on the maps

6. Run the cells - the map will open in Jupyter and your default web browser

## Notes:

Cell 4 creates a centroid column for the ngd data, which loads slightly quicker on the maps than the polygon data. And also enables a clearer visual comparison with the ab data, which is centroids.

Cell 6 creates a geometry column from the x and y coordinates provided in the ab data. The geometry column is required to display the data on the map.

##

This was made by [Lewis Jones](mailto:lewis.jones@ons.gov.uk)  as part of his apprenticeship rotation through the ONS Geospatial team in DALI.
