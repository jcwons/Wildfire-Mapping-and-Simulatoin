# Wildfire Mapping and Simulation
## Introduction
In this directory, you can find notebooks on how to calculate the affected area of wildfires (blog_post.ipynb) and how to build a fire simulation using the wildfire damage data (simulation.ipynb). 

The first notebook covers in detail how to:
* Use Google Earth Explorer to download satellite imagery
* Remove clouds and cloud shadows from images
* Calculate NDVI and the normalised burn ratio (NBR)
* Create a mask of the fire and clean the final map

The simulation notebook covers how to:
* Use Cellular Automaton Models to simulate wildfires
* include NDVI, wind and elevation
* Vectorise operations using numpy
* Optimise model parameters with Optuna
* Visualise the results in an animation

The packages used in the first notebook are mainly gdal, rasterio, xarray, numpy and geopandas to handle the geospatial data. The second file is mostly numpy for the simulation because I have written all steps of the simulations without the use of any further packages. It gives a nice introduction to running a simulation, applying vectorisation and optimisation. In the final step, I used Optuna to optimise the parameters of the model.

The required packages should all be easily installed via pip install.

## Blog Posts
There are written-up versions of the notebooks without any code explaining all the steps. The notebooks provide a detailed walkthrough on how to derive at the results.

The results of how to download and process satellite imagery for measuring wildfire damage can be found [https://jcwons.github.io/github-blogs/2025/04/24/Playing-with-Fire-Part-1-Using-Remote-Sensing-to-calculate-Wildfire-damages.html](here).

The results of the wildfire simulation can be found will be uploaded soon[](here)

## Results
The final result of the wildfire simulation was an okay representation of the actual fire, but there are a lot things to improve in this simulation.

