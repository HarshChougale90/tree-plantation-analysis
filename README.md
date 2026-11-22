# Tree Plantation Need Analysis

A web tool that scans a **5 km × 5 km area** on a real-world satellite map, measures green cover, detects land-use features and shows **where tree plantation is needed and by how much (%)**.

Project Based Learning (PBL), PVG COETM, AY 2026-27
Harshvardhan Mohan Chougale (Roll No. 5003) and Shreyash Bhosale (Roll No. 5008)

## Problem statement
To analyze the land use and green cover within a 5 km × 5 km square area using satellite imagery and AI-based image analysis, identify features such as gardens, colleges, residential areas, malls, shops and parking areas, and determine locations where tree plantation is required due to insufficient green cover.

## What it does
- Real-world satellite map (Esri World Imagery) with place search
- Scans the selected 5 km × 5 km area in a grid of blocks
- Green cover per block using the Excess Green (ExG) vegetation index
- Land-use features from OpenStreetMap: gardens, residential, colleges, malls, shops, parking
- Object counts, plantation need (%), estimated trees, and ranked priority sites
- CSV and text report download

## How to use
Open the live page, search a place, set the 5 km × 5 km area, press **Scan**, then view the plantation-need table, objects table and priority sites.
An internet connection is needed (map tiles, OpenStreetMap data, search).

## Method (summary)
1. Select study area 2. Fetch satellite imagery 3. Compute green cover (ExG) 4. Fetch land-use features (OSM) 5. Grid block analysis 6. Flag blocks below the minimum green-cover threshold 7. Rank sites and report

## Limitations
Rule-based colour-index analysis, not a trained deep-learning model. Accuracy depends on image date, shadows and OpenStreetMap completeness.

## Data and credits
Esri World Imagery, OpenStreetMap contributors (ODbL), Nominatim, Leaflet.

## License  
MIT
