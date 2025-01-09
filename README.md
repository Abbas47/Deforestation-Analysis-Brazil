# README

## Project Overview
This project is a skill assessment for the Trase Data Scientist position at the Stockholm Environment Institute. It involves analyzing spatial data to calculate deforestation and cropland-driven deforestation across Brazilian biomes using Google Earth Engine (GEE) and R/Python.

The project evaluates technical proficiency in spatial data analysis, scripting, data visualization, and report writing.

---

## Objectives
The primary objectives of this project are:
1. **Technical Analysis:** Use GEE, R, or Python to compute the following:
   - Total deforestation from 2010 to 2023 for each Brazilian biome using the Mapbiomas and Global Forest Watch (GFW) datasets.
   - Deforestation driven by cropland expansion during the same period.
2. **Visualization and Comparison:** Generate visualizations and summary statistics comparing results from the two datasets.
3. **Article Writing:** Create a concise report highlighting the methodology, findings, and potential reasons for discrepancies between datasets.

---

## Dataset Information
1. **Global Forest Watch (GFW):**
   - Provides global forest loss data.
   - Accessible through GEE: `ee.Image('UMD/hansen/global_forest_change_2023_v1_11')`

2. **Mapbiomas:**
   - Offers land use and land cover change data.
   - Accessible through GEE:
     - Deforestation asset: `ee.Image('projects/mapbiomas-public/assets/brazil/lulc/collection9/mapbiomas_collection90_deforestation_secondary_vegetation_v1')`
     - Land use/cover asset: `ee.Image('projects/mapbiomas-public/assets/brazil/lulc/collection9/mapbiomas_collection90_integration_v1')`

3. **Brazilian Biomes:**
   - Spatial layer of biomes.
   - Accessible through GEE: `ee.FeatureCollections('projects/mapbiomas-territories/assets/TERRITORIES/LULC/BRAZIL/COLLECTION9/WORKSPACE/BIOMES')`

---

## Analysis Steps
### 1. Technical Analysis
   - **Deforestation Calculation:**
     - Compute total deforestation from 2010 to 2023 for each biome using Mapbiomas and GFW.
     - Use land use/cover data to identify deforestation caused by cropland expansion.
   - **Tools Used:** Google Earth Engine (GEE), Python, or R.

### 2. Visualization and Statistical Comparison
   - Prepare summary statistics and visualizations comparing results from the two datasets.
   - Highlight key differences and trends.

### 3. Report Creation
   - Write a concise article detailing:
     - Methodology for calculating cropland-driven deforestation.
     - Comparison of findings between datasets.
     - Explanation for differences observed.

---

## Results
The outputs include:
1. Scripts for data analysis and visualization.
2. Summary statistics and graphical visualizations.
3. A 300-500 word article summarizing the findings and their implications.

---

## How to Run the Project
### Prerequisites
- Google Earth Engine account.
- Python or R installed with necessary libraries (e.g., `earthengine-api`, `pandas`, `matplotlib`, `geopandas`).

### Steps
1. Clone the repository or download the project folder.
2. Access the datasets using the specified GEE paths.
3. Run the scripts in the following order:
   - Deforestation Calculation (Script 1).
   - Cropland-driven Deforestation (Script 2).
   - Visualization and Summary Statistics (Script 3).
4. Review the generated visualizations and the written report.

---

## Dependencies and Setup Instructions
1. **Python Libraries:**
   - `earthengine-api`
   - `pandas`
   - `matplotlib`
   - `geopandas`
2. **R Libraries:**
   - `sf`
   - `ggplot2`
   - `rgee`
3. **Setup:**
   - Install required libraries.
   - Authenticate with GEE using `earthengine authenticate`.
   - Update paths in scripts as needed.

---

## Additional Information
For any questions or troubleshooting, contact: [florian.gollnow@sei.org](mailto:florian.gollnow@sei.org).


