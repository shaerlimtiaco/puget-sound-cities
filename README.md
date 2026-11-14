# Puget Sound Cities: Mapping South Puget Sound with Python

![Map of South Puget Sound cities](puget_sound_map.png)

## Overview

This project maps 14 cities in South Puget Sound, Washington, from Seattle to Tacoma, centered on Federal Way. It uses open Census data and Python to filter, reproject and measure city boundaries, and produces both a static and an interactive map.

## Data

- [U.S. Census Bureau TIGER/Line 2024: Places (Washington)](https://www2.census.gov/geo/tiger/TIGER2024/PLACE/)

## Methods

1. Loaded Washington city boundaries with GeoPandas
2. Filtered to 14 South Puget Sound cities by name
3. Reprojected from NAD83 (EPSG:4269) to Washington State Plane South, US feet (EPSG:2927), for accurate area measurement
4. Calculated each city's area in square miles
5. Created a static map (matplotlib) and an interactive web map (folium)

## Results

Federal Way covers about ___ square miles and ranks ___ in size among the 14 cities.

## Tools

Python, GeoPandas, matplotlib, folium, JupyterLab

## How to run

```
conda create -n gis -c conda-forge python=3.12 geopandas jupyterlab matplotlib folium
conda activate gis
jupyter lab
```

Then open `puget_sound.ipynb` and choose Run → Run All Cells.

## Author

Shae Limtiaco · [GitHub](https://github.com/shaerlimtiaco)