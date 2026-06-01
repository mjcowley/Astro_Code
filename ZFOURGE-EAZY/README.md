# ZFOURGE EAZY Notebook

<img src="../Images/qarg_bw_dark.png" alt="QUT Logo" width="500" />

A self-contained eazy-py notebook for computing photometric redshifts and stellar population properties for the ZFOURGE survey fields (CDFS, COSMOS, UDS). Catalogue data is downloaded automatically from Vizier; no local input files required.

Based on the eazy-py demo notebook by Gabriel Brammer (University of Copenhagen).
eazy-py: https://github.com/gbrammer/eazy-py

## Key Features

- **Field selection** - Switch between CDFS, COSMOS, and UDS with a single toggle
- **Automated catalogue download** - Retrieves ZFOURGE photometry directly from Vizier (Straatman et al. 2016)
- **Iterative zeropoint corrections** - Derives per-filter zeropoint offsets to improve photometric accuracy
- **Photometric redshift fitting** - Full eazy-py pipeline including priors and P(z) computation
- **Stellar population properties** - Stellar masses, SFRs, rest-frame colours, and dust attenuation derived from spline SED templates
- **Interactive visualisation** - Plotly/Dash explorer for browsing SEDs and catalogue properties
- **UVJ diagram** - Rest-frame colour classification of star-forming and quiescent galaxies coloured by sSFR

## Files

- `eazy_zfourge.ipynb` - Full pipeline from catalogue download to visualisation
- `zfourge.cdfs.vizier.translate.csv` - Filter translate file for CDFS
- `zfourge.cosmos.vizier.translate.csv` - Filter translate file for COSMOS
- `zfourge.uds.vizier.translate.csv` - Filter translate file for UDS

## Output Files

- `zfourge.{field}.zspec.vizier.csv` - Input catalogue
- `zfourge.{field}.zout.fits` - Redshifts and stellar population parameters
- `zfourge.{field}.zphot.zeropoint` - Derived zeropoint corrections
- `zfourge.{field}.h5` - Full fit data for SED plotting
- `zfourge.{field}.output.fits` - Exported catalogue for further analysis

## Requirements

- Python 3.10+
- `eazy`
- `grizli`
- `astroquery`
- `dust_attenuation`
- `pandas`
- `numpy`
- `astropy`
- `matplotlib`
- `ipywidgets`
- `dash`

All dependencies are installed automatically by Cell 1 of the notebook.

## Running the Notebook

The recommended option for users new to Python is Google Colab - no local installation required. Open the notebook in Colab, run Cell 1, and all dependencies will be installed automatically.

For local use, ensure you have Python 3.10 or later and Jupyter installed before opening the notebook.

## References

Straatman et al. (2016), ApJ, 830, 51
