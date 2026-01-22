# Biodiversity-data-challenge
Predicting frog species presence using satellite climate data 
About
🐸 Predicting frog species presence using satellite climate data 🌍

This project demonstrates the power of combining biodiversity data with satellite-derived climate information to predict species distributions. Using machine learning and geospatial analysis, we predict frog presence in southeastern Australia based on 14 TerraClimate variables from Microsoft's Planetary Computer.

Key Features:

📊 6,314 training samples with 14 climate variables
🌡️ TerraClimate data integration (1958-present)
🗺️ Geospatial analysis for precise location-based predictions
🤖 Binary classification with Random Forest
📈 Comprehensive model evaluation and validation
🎓 Educational focus for environmental data science
Perfect for learning satellite data analysis, geospatial machine learning, and biodiversity modeling!

Project Overview
This project focuses on predicting the presence of frog species in southeastern Australia using climate variables from the TerraClimate dataset. The goal is to build a binary classification model that can accurately predict whether frogs are present at specific geographic locations based on environmental factors.

🎯 Objective
The primary objective is to develop a machine learning model that predicts frog species presence using TerraClimate variables extracted from the Microsoft Planetary Computer data catalog. The model uses monthly climate and climatic water balance data from 1958 to the present to understand the relationship between environmental conditions and frog habitat suitability.

📊 Datasets
1. Frog Presence Data
Source: Global Biodiversity Information Facility (GBIF)
Coverage: Southeastern Australia
Time Period: November 2017 to November 2019 (2 years)
Format: CSV with columns:
Latitude: Geographic latitude coordinates
Longitude: Geographic longitude coordinates
Occurrence Status: Binary indicator (1 = presence, 0 = absence)
2. Climate Data (TerraClimate)
Source: Microsoft Planetary Computer
Coverage: Global terrestrial surfaces
Time Period: 1958 to present
Resolution: ~4-km (1/24th degree) spatial resolution
Variables: 14 climate variables including:
aet: Actual Evapotranspiration
def: Climate Water Deficit
pdsi: Palmer Drought Severity Index
pet: Potential Evapotranspiration
ppt: Precipitation
q: Runoff
soil: Soil Moisture
srad: Downward Shortwave Radiation Flux
swe: Snow Water Equivalent
tmax: Maximum Temperature
tmin: Minimum Temperature
vap: Vapor Pressure
vpd: Vapor Pressure Deficit
ws: Wind Speed
