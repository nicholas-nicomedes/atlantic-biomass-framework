# Atlantic Forest Biomass Estimation Framework

![Status: Work in Progress](https://img.shields.io/badge/Status-Work_in_Progress-yellow)
![License: MIT](https://img.shields.io/badge/License-MIT-blue)
![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue)
![R Support](https://img.shields.io/badge/R-Supported-blue)

A reproducible computational framework for estimating above-ground forest biomass in the Atlantic Forest of Brazil. 

This project integrates spaceborne data from **ESA's BIOMASS P-band SAR mission** with high-resolution **drone LiDAR** and **multispectral imagery** to bridge the methodological gap between emerging global satellite observations and high-resolution local measurements.

## Project Overview
This repository hosts the computational workflows developed as part of a PhD research project in Environmental Sciences at UNESP, Brazil. It sits at the intersection of geoprocessing, remote sensing, spatial statistics, and machine learning.

The overarching goal is not just to estimate biomass in a single study area, but to develop **reusable geospatial processing, feature-engineering, modeling, and validation workflows** that can support open-source forest monitoring, carbon-stock assessment, and future BIOMASS applications globally.

## Methodology & Tech Stack

### Data Fusion
*   **ESA BIOMASS P-band SAR:** Macro-scale observations and structural canopy parameters.
*   **UAV LiDAR Point Clouds:** High-resolution structural data utilized as ground-truth proxy for validation.
*   **Multispectral Imagery:** Geospatial variables and vegetation indices (NDVI, SAVI, EVI, NDRE, GNDVI).

### Machine Learning Modeling
Evaluating the transferability and robustness of relationships between structural forest variables and biomass using:
*   Random Forest
*   Support Vector Machines (SVM)
*   XGBoost

### Architecture
*   `src/preprocessing/`: Spatial alignment, resampling, and feature engineering for LiDAR and SAR fusion.
*   `src/modeling/`: ML pipeline development and hyperparameter tuning.
*   `src/validation/`: Spatial cross-validation and error diagnostics.

## Current Status
> **Note:** This project is currently in the initial data collection and methodological design phase of a doctoral research effort. 

Active development is focused on designing the spatial preprocessing pipelines. As the project matures, research scripts will be refactored into cleaner, modular, and reusable components available in this repository.

## License
This project is licensed under the MIT License - seeing as the ultimate goal is to provide a reproducible research resource for the Earth observation and environmental modeling community.
