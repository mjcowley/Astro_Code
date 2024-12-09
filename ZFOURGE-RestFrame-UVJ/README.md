# UVJ Diagram and sSFR Analysis

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="QUT Logo" width="500" />

This repository contains Python code for querying, processing, and visualising galaxy data to create **UVJ diagrams** and analyse the **specific star formation rates (sSFR)** of galaxies. The project retrieves data from **Vizier** for the COSMOS field, filters galaxies by specific criteria (redshift, stellar mass, etc.), and then visualises galaxy populations on the UVJ diagram. Additionally, galaxies are coloured based on their sSFR to distinguish between star-forming and quiescent galaxies.

## Key Features

- **Data Retrieval**: Query multiple Vizier catalogs (rest-frame fluxes, stellar mass, redshift, and sSFR) for galaxies in the **COSMOS** field.
- **UVJ Diagram**: Plot the rest-frame U-V vs V-J colours to classify galaxies as star-forming, quiescent, or dusty.
- **sSFR Analysis**: Colour galaxies on the UVJ diagram based on their specific star formation rate (sSFR), allowing for a more detailed classification.
- **Data Filtering**: Apply filters to select galaxies within a specific redshift range (0.5 < z < 3.5) and stellar mass (lmass > 10).
- **Data Masking**: Mask the data using the "use" flag to ensure you are working with a standard selection of galaxies.

## Files

1. **UVJ_Diagram_Analysis.ipynb**: Jupyter notebook containing the full code for querying, processing, and visualising the data, as well as generating the UVJ diagram.

## Requirements

- Python 3.x
- `astroquery`
- `matplotlib`
- `pandas`
- `numpy`
