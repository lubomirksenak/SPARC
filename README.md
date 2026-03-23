# SPARC
**S**peckle **P**rocessing **A**nd **R**adar **C**lassification

⚠️ This repository is currently under development.

The code and documentation are being prepared.  
More details will be available soon

This repository contains the code and supporting materials used in the study:
**"Terrain-dependent Effects of SAR Speckle Filtering on Land Cover Classification Using Sentinel-1"** on adress: (TBA after article acceptance).

## 🔍 Description

SPARC provides an experimental workflow for evaluating how SAR speckle filtering influences binary land-cover classification using Sentinel-1 GRD imagery. The repository focuses on five contrasting areas of interest in eastern Slovakia: mountain, forest, urban, cropland, and water.

The workflow combines:
- Sentinel-1 preprocessing outputs,
- comparison of multiple speckle filters,
- Lee Sigma window-size sensitivity analysis,
- extraction of SAR quality metrics,
- supervised classification using SVM, Random Forest, and Histogram-based Gradient Boosting.

The scripts is implemented in **Python** 

## Study scope

According to the manuscript, the study evaluates eight speckle filtering algorithms across five terrain types using Sentinel-1 GRD data, with classification tested under VV, VH, and dual-polarization configurations. The analysis uses repeated balanced sampling and reports OA, F1, and Cohen’s kappa together with PSNR, MSE, SSIM, and ENL.

## 🔍 Description

SPARC provides an experimental workflow for evaluating how SAR speckle filtering influences binary land-cover classification using Sentinel-1 GRD imagery. The repository focuses on five contrasting areas of interest in eastern Slovakia: mountain, forest, urban, cropland, and water.

## 🛰️ Data Sources

- **Sentinel-1 GRD (IW mode, VV/VH polarization)** - Copernicus Programme (via Copernicus Data Space Ecosystem / Sentinel Hub API
- **ESA WorldCover 2021** - European Space Agency (via Microsoft Planetary Computer STAC API using pystac-client)
- **Copernicus DEM GLO-30** - Copernicus Programme (via Microsoft Planetary Computer STAC API using pystac-client)
- **Optional local GeoTIFF inputs** - generated within this study workflow

## ⚙️ Methodology Overview

- Prepare preprocessed Sentinel-1 VV and VH backscatter rasters
- Organize outputs by AOI and filtering method
- Build reference masks from ESA WorldCover and Copernicus DEM
- Sample balanced train/test points
- Extract backscatter and texture features
- Run classification benchmarks
- Compare performance across filters, polarizations, terrains, and Lee Sigma window sizes
- Compute SAR image quality metrics for selected filtered outputs

## 📁 Structure

## 📊 Outputs

- Classification metrics tables
- Confusion matrices
- Best-model maps
- Filter comparison summaries
- Speckle quality metrics

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🔗 Citation

If you use this script or data in your research, please cite the corresponding publication:
- Kseňak, Ľ.; Bartoš, K.; Pukanská, K. Terrain-dependent Effects of SAR Speckle Filtering on Land Cover Classification Using Sentinel-1 (TBA after article acceptance)

## 📬 Contact

For questions or collaboration, contact:  
**Dr. Ľubomír Kseňak**  
Technical university of Košice, Slovakia  
lubomir.ksenak@tuke.sk
