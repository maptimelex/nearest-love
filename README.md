# Where is your nearest love?

A mapping project for Maptime Lex Valentine's Day Special.

![need map love](images/need-map-love.png)

## Valentine's Day Mapping

This project provides a high-level overview of a geospatial data project seeking to identify and map place names within the US containing Valentine's Day-related terms (such as "love" or "heart").

While the intent of maptimeLex event is fun (and perhaps a bit silly), we'll be introducing and covering the following process.

### 1. Data wrangling and transformation using Python within a Jupyter Notebook

Data source: [US Domestic Geographic Names Database](https://www.usgs.gov/core-science-systems/ngp/board-on-geographic-names/download-gnis-data).

Recommended: First create a new virtual environment and launch the .pynb Jupyter Notebook(s) within that. An example of the installed Python packages is here: [./notebooks.bio-env.txt](./notebooks.bio-env.txt).

The love_mapping.ipynb Notebook provides some preliminary loading, exploration, filtering, and transformation of the dataset. The key Python libraries employed are:

- [pandas](https://pandas.pydata.org/): used for quickly reading the tabular dataset into the Notebook, analyzing, and filtering
- [geopandas](https://geopandas.org/): used for quickly converting a pandas DataFrame (of tabular data) into a GeoDataFrame (with a geometry column attribute)
- [pysal](https://pysal.readthedocs.io/en/latest/index.html): used to analyze the filtered points and create Voronoi polygons

The standard-library-version.ipynb Notebook tests a similar process for filtering data and writing the resultant point features to GeoJSON.

### 2. Quick plotting and analysis within a web map
