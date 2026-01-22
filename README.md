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

**Getting Started**
Prerequisites
Install the required Python packages:

pip install numpy pandas matplotlib seaborn xarray geopandas rasterio
pip install scikit-learn joblib tqdm pystac-client planetary-computer

Running the Analysis

1.Open the main notebook:

jupyter notebook Biodiversity_Challenge_Group6.ipynb

2.Follow the workflow:

Load and explore the training data
Process TerraClimate variables
Build and train the machine learning model
Evaluate model performance
Generate predictions for validation dataset

3.For TerraClimate data processing:

jupyter notebook TerraClimate.ipynb

📈 **Model Performance**

The current implementation demonstrates:

Binary Classification: Predicting frog presence (1) vs absence (0)
Feature Selection: Using 14 TerraClimate variables as predictors
Geographic Coverage: Southeastern Australia region
Temporal Coverage: 2-year period (2017-2019)

**🎓 Educational Purpose**

This project serves as a learning tool for:

Satellite Data Analysis: Working with TerraClimate datasets
Geospatial Machine Learning: Combining location data with environmental variables
Biodiversity Modeling: Understanding species-environment relationships
Real-world Applications: Practical experience with ecological data science

**🔍 Key Features**

Comprehensive Climate Variables: 14 different environmental factors
Geospatial Integration: Precise location-based climate extraction
Scalable Architecture: Can be extended to other species or regions
Reproducible Workflow: Complete data processing and modeling pipeline
Validation Framework: Structured approach for model evaluation

**📝 Output Format**
The model generates predictions in the following format:
Latitude,Longitude,Occurrence Status
-33.121788,150.320746,1
-36.592011,148.172262,0
...

🤝 **Contributing**

This is an educational project designed for learning purposes. Students are encouraged to:

Experiment with different climate variables
Try alternative machine learning algorithms
Explore additional data preprocessing techniques
Extend the analysis to other geographic regions

**📚 References**

TerraClimate Dataset Documentation
Global Biodiversity Information Facility
Microsoft Planetary Computer

**📄 License**
This project is for educational purposes. Please refer to the original data sources for licensing information.

**🎯 Final Findings and Results**

**Model Performance Summary**
Our Random Forest model achieved the following performance metrics:

In-Sample Performance (Training Data)
Overall Accuracy: 97%
Precision: 98% (Class 0), 97% (Class 1)
Recall: 95% (Class 0), 99% (Class 1)
F1-Score: 97% (Class 0), 98% (Class 1)
Out-of-Sample Performance (Test Data)
Overall Accuracy: 75%
Precision: 70% (Class 0), 78% (Class 1)
Recall: 65% (Class 0), 82% (Class 1)
F1-Score: 67% (Class 0), 80% (Class 1)

**Key Insights**

Feature Importance Analysis

The Random Forest model identified the following climate variables as most important for predicting frog presence:

Precipitation (ppt) - 10.95% importance
Actual Evapotranspiration (aet) - 10.66% importance
Downward Shortwave Radiation (srad) - 9.67% importance
Potential Evapotranspiration (pet) - 9.41% importance
Climate Water Deficit (def) - 9.21% importance
Vapor Pressure (vap) - 9.03% importance
Palmer Drought Severity Index (pdsi) - 7.68% importance

Environmental Factors Driving Frog Distribution

Water Availability: Precipitation and evapotranspiration are the most critical factors, indicating frogs prefer areas with adequate water supply

Solar Radiation: Moderate levels of solar radiation support frog habitats, likely through vegetation growth and temperature regulation

Climate Balance: The balance between potential and actual evapotranspiration suggests frogs prefer areas with stable moisture conditions

Drought Conditions: The Palmer Drought Severity Index shows moderate importance, indicating frogs are sensitive to drought conditions

**Model Architecture**

Algorithm: Random Forest Classifier with 100 estimators
Max Depth: 50 (to prevent overfitting)
Feature Selection: 7 most important climate variables
Preprocessing: Median imputation + MinMaxScaler
Data Split: 70% training, 30% testing with stratification

**Validation Results**

The model successfully generated predictions for 2,000 validation locations across southeastern Australia, providing binary presence/absence predictions based on the learned environmental relationships.

**Environmental Implications**

Habitat Suitability: The model can identify areas with suitable environmental conditions for frog species

Climate Change Impact: The model framework can be adapted to assess how climate change might affect frog distributions

Conservation Planning: Results can inform habitat protection and restoration efforts

Biodiversity Monitoring: The approach can be extended to other species and regions

**Technical Achievements**

Geospatial Integration: Successfully combined point location data with raster climate data

Feature Engineering: Identified the most predictive climate variables

Model Optimization: Achieved good balance between performance and generalization

Scalable Framework: The methodology can be applied to other species and regions

**Future Work**

Model Enhancement: Explore ensemble methods and deep learning approaches

Temporal Analysis: Incorporate seasonal and interannual climate variations

Multi-species Modeling: Extend to multiple frog species simultaneously

Climate Change Scenarios: Model future distributions under climate change projections

Habitat Connectivity: Incorporate landscape connectivity factors

Note: This project demonstrates the application of machine learning techniques to biodiversity conservation and environmental science, providing valuable insights into species-environment relationships. The final model successfully predicts frog presence with 75% accuracy on unseen data, highlighting the potential of satellite-derived climate data for biodiversity modeling and conservation planning.
