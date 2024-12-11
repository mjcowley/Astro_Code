# Vizier ZFOURGE Querying and Data Processing

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="QUT Logo" width="500" />

This repository contains Python code for querying and processing ZFOURGE data from the **Vizier** database. The ZFOURGE Survey provides a comprehensive collection of photometric data for galaxies in multiple fields: **CDFS**, **COSMOS**, and **UDS**. This code demonstrates how to retrieve and process catalogs from Vizier, perform data selection, and visualise key astrophysical parameters like stellar mass and redshift.

## Key Features

- **Query ZFOURGE Data** - Retrieve data from multiple ZFOURGE catalogs including photometric and stellar population data.
- **Data Selection** - Select galaxies based on the "use" flag, as detailed in the Straatman et al. 2016 paper, to ensure a standard selection of galaxies.
- **Data Visualisation** - Plot mass vs redshift, both for the entire catalog and after applying the selection criteria.
- **Data Masking** - Mask the data using the "use" flag to ensure you are working with a standard selection of galaxies.

## Files

1. **ZFOURGE-VizieR-Import.ipynb** - Jupyter notebook containing the full code to query, process, and visualise the ZFOURGE data.

![SED](https://mjcowley.github.io/qut/Images/uvj.png)

## Requirements

- Python 3.x
- `astroquery`
- `matplotlib`
- `pandas`
- `numpy`
