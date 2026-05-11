# Hyperspectral Socioeconomic Mapping

This repository contains the code, preprocessing workflows, representative sample datasets, and example outputs used in the study:

"Mapping Urban Socioeconomic Disparities Using Remote Sensing Hyperspectral Data"

---

# Repository Structure

- `notebooks/`
  - PRISMA preprocessing workflow
  - PCA and boxplot analysis
  - Classification workflow

- `sample_data/`
  - Representative labeled coordinate datasets used for model training/testing

- `results/`
  - Representative PCA plots, scree plots, and classification outputs

- `docs/`
  - Additional workflow documentation

---

# Data Sources

## PRISMA Hyperspectral Data

PRISMA hyperspectral imagery is freely available from the Italian Space Agency after user registration:

https://prisma.asi.it/

The PRISMA scenes corresponding to the acquisition dates used in this study can be searched and downloaded from the official portal.

## Landsat 8 Data

Landsat 8 imagery is publicly available from the USGS EarthExplorer platform:

https://earthexplorer.usgs.gov/

---

# Socioeconomic Reference Data

The socioeconomic labels were derived using secondary data obtained from:

- Department of Stamps and Registration, Karnataka  
  https://kaveri.karnataka.gov.in/landing-page

- Directorate of Registration and Stamp Revenue, Finance Department, Government of West Bengal  
  https://wbregistration.gov.in/MV/mv_aprt.aspx

Property guidance values were categorized into income-based socioeconomic classes for Bangalore and Kolkata.

---

# Reproducibility Workflow

1. Download PRISMA and Landsat imagery from the official portals
2. Convert PRISMA `.he5` files into GeoTIFF format
3. Generate spectral features and PCA components
4. Perform socioeconomic class separability analysis
5. Train machine learning classifiers
6. Evaluate classification performance and generate outputs

---

# Notes

This repository contains representative sample datasets and workflows necessary for reproducibility. Large raw satellite datasets are publicly available from the official data providers listed above.
