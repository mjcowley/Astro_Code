# CIGALE Model for Spectral Energy Distribution (SED) Fitting

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="CIGALE" width="500" />

Python code for running the CIGALE model to fit Spectral Energy Distributions (SEDs) of galaxies. This notebook includes:
- Running the CIGALE model to derive physical properties like star formation rates (SFR) and dust attenuation from multi-band flux measurements.
- Using CIGALE to model galaxies' spectral energy distributions by fitting observed photometry with theoretical models.

## Files

1. **sdss_qso.txt** - Example input data file containing galaxy flux measurements and redshift values.
2. **pcigale.ini** - Configuration file for the CIGALE model, including data file and SED modules.
3. **pcigale.ini.spec** - Specification file for CIGALE, generated during the configuration step.
4. **best_model.fits** - Output file containing the best-fitting model's **SED** and derived parameters.

## Key Features

- **SED Fitting** - Fit the observed galaxy photometry to theoretical models of stellar population synthesis and dust attenuation.
- **Model Components** - Includes various modules for star formation history, stellar population modeling, nebular emission, and dust attenuation.
- **Model Output** - Generate the best-fitting SED and other model outputs such as star formation rates (SFRs) and flux densities in different bands.
- **Log-Log SED Plot** - Visualize the fitted **SED** using a **log-log scale** plot to inspect the model’s performance across wavelengths.

## Requirements

- Python 3.x
- `matplotlib`
- `astropy`
- `numpy`
- `subprocess`

## Setup and Usage

1. **Clone the Repository**:

   Clone this repository to get started:

   ```bash
   git clone https://github.com/YOUR_USERNAME/cigale-sed-model.git
   cd cigale-sed-model
