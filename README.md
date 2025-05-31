# BoundaryBackend_extractor
# Geospatial Data Extraction Framework

A modular geospatial data extraction system supporting Landsat and Sentinel datasets. Designed for easy extension and integration into ODC-compatible pipelines.

## Requirements

- Python 3.11
- Conda
- `python-dotenv` for environment variable management

## Setup

Create a conda environment:
bash
conda env create -f environment.yml

Activate the environment:
bash
conda activate geo_env_311

Add your USGS credentials to a .env file:
LANDSAT_USERNAME=your_username
LANDSAT_API_KEY=your_api_key

Notes
Extraction output (raw, preprocessed, validated) is saved to extracted_data/.
Extend with other extractors (e.g., Sentinel, DEM) by inheriting from GeospatialDataExtractorBase.
