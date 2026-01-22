# Biodiversity-data-challenge
Predicting frog species presence using satellite climate data 
About
🐸 Predicting frog species presence using satellite climate data 🌍
redicting Frog Species Presence Using Satellite Climate Data 🌍

This project demonstrates how biodiversity data and satellite-derived climate variables can be combined to predict species distributions using machine learning and geospatial analysis.

We model frog species presence in southeastern Australia using TerraClimate variables accessed via Microsoft’s Planetary Computer, highlighting practical applications of environmental data science.

🔍 Project Overview

Understanding how climate influences species habitats is critical for conservation and environmental planning.
This project builds a binary classification model that predicts whether frogs are present at specific geographic locations based on historical and environmental conditions.

The analysis integrates biodiversity occurrence data with high-resolution climate data, enabling location-based predictions.

🎯 Objective

The primary objective is to develop a machine learning model that predicts frog species presence (1 = present, 0 = absent) using climate variables extracted from the TerraClimate dataset.

The model leverages monthly climate and climatic water balance data (1958–present) to capture long-term environmental patterns influencing habitat suitability.

⭐ Key Features

📊 6,314 training samples with 14 climate variables

🌡️ TerraClimate data integration (1958–present)

🗺️ Geospatial analysis for location-based predictions

🤖 Binary classification using Random Forest

📈 Comprehensive model evaluation & validation

🎓 Educational focus on environmental & geospatial data science

📊 Datasets
1️⃣ Frog Presence Data

Source: Global Biodiversity Information Facility (GBIF)

Region: Southeastern Australia

Time Period: November 2017 – November 2019

Format: CSV

Key Fields:

Latitude – Geographic latitude

Longitude – Geographic longitude

Occurrence Status – Binary indicator (1 = presence, 0 = absence)

2️⃣ Climate Data – TerraClimate

Source: Microsoft Planetary Computer

Coverage: Global terrestrial surfaces

Time Period: 1958 – Present

Spatial Resolution: ~4 km (1/24°)

Climate Variables (14):

aet – Actual Evapotranspiration

def – Climate Water Deficit

pdsi – Palmer Drought Severity Index

pet – Potential Evapotranspiration

ppt – Precipitation

q – Runoff

soil – Soil Moisture

srad – Downward Shortwave Radiation

swe – Snow Water Equivalent

tmax – Maximum Temperature

tmin – Minimum Temperature

vap – Vapor Pressure

vpd – Vapor Pressure Deficit

ws – Wind Speed

🧠 Modeling Approach

Problem Type: Binary Classification

Algorithm: Random Forest

Inputs: 14 climate variables + geospatial coordinates

Output: Frog presence probability

The model captures nonlinear relationships between climate variables and frog habitat suitability.

📌 Use Cases & Learning Outcomes

This project is ideal for learning:

Satellite & climate data analysis

Geospatial machine learning

Environmental & biodiversity modeling

Feature engineering with climate datasets

Applied classification modeling

🚀 Why This Project Matters

This work demonstrates how open satellite data and machine learning can support ecological research, conservation efforts, and climate-driven decision-making.

## 📂 Project Structure

biodiversity_data_Challenge/
│
├── Biodiversity_Challenge_Group6.ipynb      # Main analysis notebook

├── TerraClimate.ipynb                       # TerraClimate data processing

├── Training_Data.csv                        # Training dataset (6,314 samples)

├── Validation_Template.csv                  # Validation dataset (2,002 samples)

├── Biodiversity_Challenge_Overview.pdf      # Project overview document

├── Group 6 - Value Case.pdf                 # Value case analysis

├── Group 6 - Project Presentation.pptx      # Final project presentation

└── README.md                                # Project documentation

**Methodology**

Data Processing Pipeline
Data Loading: Load frog presence data and TerraClimate variables
Geospatial Extraction: Extract climate values for each frog observation location
Feature Engineering: Combine frog presence data with climate variables
Data Preprocessing: Handle missing values and normalize features
Model Training: Train binary classification model
Evaluation: Assess model performance using classification metrics
Validation: Predict on new locations using validation template

**Machine Learning Approach**
Algorithm: Random Forest Classifier
Preprocessing:
Missing value imputation (median)
Feature scaling (MinMaxScaler)
Evaluation Metrics: Precision, Recall, F1-Score, Accuracy
Cross-validation: Train-test split (70-30)
