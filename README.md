# Roadkill Prediction Project

## Overview
This project aims to predict wildlife-vehicle collisions by analyzing environmental characteristics extracted from satellite imagery along road segments. Using machline learning techniques and geospatial analysis, we combine road segment data with Landsat imagery to identify high-risk areas for wildlife-vehicle collisions.

## Features
- Satellite Imagery Collection
  - Automated collection of Landsat Imagery (5,7,and 8)
  - Multi-buffer zone analysis
  - Fall season (September-October) imagery focus
  - 10m resolution output
 
- Environmental Feature Extraction
  - Sprectral Indices (NDVI, NDWI, NDBI)
  - Band statistics and texture features
  - Multi-scale environmental analysis
  - Feature validation and quality control
 
- Band Segment Processing
  - Aggregation from 25m to 100m/200m segments
  - Spatial continuity validation
  - Buffer zone optimization
  - Connectivity analysis

- RandomForest Analysis
  - RandomForestClassfier Models
  - Determining best aggregation and buffer size combination
  - Using prediction error values to measure

 ## Installation 
 1. Clone the repository and install required packages
 ```bash
git clone https://github.com//grantjackson580//wildlife-collision-prediction
cd wildlife-collision-prediction
pip install -r requirements.txt
```
2. Create and activate virtual environment
```bash
python -m venv env
source env/bin/activate # On Windows: env/Scripts/activate
```
3. Set up Google Earth Engine authentication
```bash
earthengine authenticate
```
4. (Notes)
  - Must run imagery collection on aggregated .gpkg files
  - Extract features from specific file directory (contains .tif files)
  - Then use Dataset Merging to combine extracted features .csv with data from aggregated .gpkg files

## CURRENTLY IN PROGRESS WITH THIS PROJECT

