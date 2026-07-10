# 🔥 Forest Fire Prediction in Algeria & Tunisia

A complete machine learning and geospatial data mining pipeline for predicting forest fire occurrence in Algeria and Tunisia using multi-source environmental datasets.

---

## 📌 Overview

Forest fires are a major environmental challenge that causes vegetation loss, biodiversity degradation, and significant economic damage. This project aims to predict forest fire occurrence by integrating heterogeneous geospatial datasets and applying both supervised and unsupervised machine learning algorithms.

The project covers the complete workflow, including:

- Data acquisition
- Data preprocessing
- Spatial data integration
- Feature engineering
- Machine learning
- Model evaluation
- Result visualization

This project was developed as part of the **Data Mining** course (M2 Artificial Intelligence and Data Science, USTHB, 2025–2026).

---

## 🚀 Features

- Multi-source geospatial data integration
- Spatial interpolation using Inverse Distance Weighting (IDW)
- Complete preprocessing pipeline
- Feature engineering
- Handling class imbalance
- Exploratory Data Analysis (EDA)
- From-scratch implementation of several machine learning algorithms
- Comparison with Scikit-learn implementations
- Supervised and unsupervised learning
- Model evaluation and visualization

---

## 📊 Data Sources

The datasets are **not included** in this repository due to their size and licensing restrictions.

### 🔥 Fire Dataset

Source: NASA FIRMS (VIIRS NOAA-20)

https://firms.modaps.eosdis.nasa.gov/country/

Selection:

- Instrument: VIIRS NOAA-20
- Year: 2024
- Countries:
  - Algeria
  - Tunisia

---

### 🌦 Climate Dataset

Source: WorldClim 2.1 + CRU TS

https://worldclim.org/data/monthlywth.html

Variables used:

- Minimum temperature
- Maximum temperature
- Precipitation

Period:

2020–2024

Resolution:

5 arc-minutes (~10 km)

---

### 🏔 Elevation Dataset

Source: GMTED2010

https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/topo/downloads/GMTED/Grid_ZipFiles/be15_grd.zip

---

### 🌱 Land Cover Dataset

Algeria

https://data.apps.fao.org/catalog/iso/0e958049-2a0a-4935-83c8-af78626068fc

Tunisia

https://data.apps.fao.org/catalog/iso/d0ba96c7-786c-4f3f-bbd9-e427b3b23d2d

---

### 🌍 Soil Dataset

Source: FAO Harmonized World Soil Database (HWSD v2.0)

https://www.fao.org/soils-portal/data-hub/soil-maps-and-databases/harmonized-world-soil-database-v20/en/

Layer used:

- D1 (0–20 cm)

Main attributes:

- Sand
- Silt
- Clay
- Organic Carbon
- Bulk Density
- Soil pH
- Total Nitrogen
- CEC
- Electrical Conductivity
- Gypsum
- and other physicochemical properties.

---

## 🛠 Data Processing Pipeline

The project follows the workflow below:

```
Raw Geospatial Data
        │
        ▼
Data Collection
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Spatial Data Integration
        │
        ▼
Class Balancing
        │
        ▼
Machine Learning
        │
        ▼
Evaluation & Visualization
```

Main preprocessing tasks include:

- Duplicate removal
- Missing value imputation
- Outlier detection
- Feature scaling
- Label encoding
- Raster clipping
- Raster-to-point conversion
- Spatial interpolation (IDW)
- Spatial joins
- Dataset merging

---

## 🤖 Machine Learning Models

### Supervised Learning

Implemented from scratch:

- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Balanced Random Forest

Compared with:

- Scikit-learn implementations

---

### Unsupervised Learning

Implemented from scratch:

- K-Means
- DBSCAN
- CLARANS

Compared with optimized Scikit-learn implementations whenever applicable.

---

## 📈 Evaluation

Classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Balanced Accuracy

Clustering metrics:

- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index

---

## 💻 Technologies

- Python
- NumPy
- Pandas
- GeoPandas
- Rasterio
- Shapely
- SciPy
- Scikit-learn
- Matplotlib
- Seaborn

---



## 📌 Results

Some notable results include:

| Model | Performance |
|--------|-------------|
| KNN | 98.33% Accuracy |
| Random Forest | 98.09% Accuracy |
| Balanced Random Forest | Improved minority-class prediction |
| K-Means | Best Silhouette Score (0.594) |
| CLARANS | Robust medoid-based clustering |
| DBSCAN | Density-based clustering analysis |

---

## ⚠️ Dataset Availability

The datasets are **not included** in this repository because they are publicly available from external providers and are subject to their respective licenses.

After downloading the datasets from the links above, place them inside the `data/` directory before running the project.

---

## Author

**Afaf Farah Zenaini**

Master's Student in Intelligent Computer Systems
