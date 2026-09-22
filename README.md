# 🌴 Sarawak Tropical Forest & Land Cover Classifier

**🚀 Live Interactive Web App:** [Launch the App](YOUR_GEE_APP_URL_HERE)  
** View Source Code:** [Open in Google Earth Engine](https://code.earthengine.google.com/?scriptPath=users%2Fazaleakamellia%2FSarawakLandCoverClassifier) *(Replace with your actual script link)*  
**Author:** Azalea Kamellia Abdullah, Gs.  
**Domain:** Applied Vegetation Remote Sensing, Tropical Land Cover Classification, Natural Capital Accounting  

##  Overview
This repository contains the methodology and source code for an interactive, cloud-based land cover classification tool tailored for tropical environments like Sarawak, Malaysia. Built entirely on the **Google Earth Engine (GEE)** platform, this web application allows environmental consultants, researchers, and ESG auditors to perform on-the-fly, multi-class land cover classification without requiring local computational resources.

## 🧠 The Cutting-Edge Methodology: Optical + SAR Fusion
Tropical regions suffer from persistent cloud cover, making traditional optical-only classification unreliable. This tool addresses that critical gap by offering an **Optical + Synthetic Aperture Radar (SAR) Fusion** approach:
1. **Optical Data:** Harmonized Sentinel-2 Surface Reflectance for rich spectral detail (NDVI, NBR).
2. **SAR Data:** Sentinel-1 C-band radar (VV/VH polarization). Radar penetrates clouds and is highly sensitive to surface structure, making it exceptionally effective at distinguishing the smooth, uniform texture of agriculture (e.g., oil palm) from the complex, rough canopy of natural tropical forest.
3. **Machine Learning:** A Random Forest classifier ingests these fused features to deliver high-confidence, multi-class land cover maps.

## 🛠️ How to Use the Live App
1. **Launch the App:** Click the "Launch the App" link at the top of this README.
2. **Define AOI:** Use the native GEE drawing tools (left toolbar) to sketch your project boundary, then click "Set Drawn Geometry as AOI" in the sidebar. Alternatively, load a shapefile directly from your GEE Assets.
3. **Configure Parameters:** Select your date range (dry season recommended), choose your sensor (Optical only, or Optical + SAR fusion).
4. **Run & Export:** Click "RUN CLASSIFICATION". The app will process the data in the cloud and display the results. Use the "Export to Drive" button to download the classified GeoTIFF for use in QGIS or ArcGIS Pro.

## 📚 Scientific Foundation & Validation
The methodology underpinning this tool is grounded in peer-reviewed remote sensing practices and applied directly to my MPhil research and industry projects:
- **Abdullah, A. K., et al. (2021).** Deep forest cover classification of consecutive Landsat imageries over Borneo. *Warta Geologi Newsletter*, 47(1), 71.
- Integration of SAR texture metrics for tropical forest/agriculture separation aligns with current best practices in *ISPRS Journal of Photogrammetry and Remote Sensing*.

## 📬 Contact & Commercial Licensing
This tool is showcased as a proof-of-concept for applied geospatial methodology. For bespoke development, custom training data integration, or commercial enterprise licensing for proprietary workflows, please contact:  
📧 azaleakamellia.a@gmail.com | 🌐 [azaleakamellia.github.io](https://azaleakamellia.github.io)
