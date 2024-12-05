# Luminosity Function Fitting with Schechter Model

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="QARG" width="500" />

Python code for fitting a **Schechter function** to the corrected luminosity function of galaxies. The example includes the following steps:

- Querying SDSS for galaxy data with redshifts between 0.015 and 0.05.
- Applying extinction corrections to apparent magnitudes to compute absolute magnitudes.
- Correcting the luminosity function using the 1/Vmax method.
- Fitting the corrected luminosity function with the Schechter function model.

## Files

1. **SDSS_query.ipynb**: Jupyter notebook containing code to retrieve and process SDSS data for galaxies.

## Key Features

- **Data Querying**: Retrieve SDSS galaxy data based on redshift and location criteria.
- **Attenuation Corrections**: Apply extinction corrections to apparent magnitudes using SDSS data.
- **Luminosity Function Calculation**: Calculate the luminosity function for galaxies using the 1/Vmax method.
- **Schechter Function Fitting**: Fit a Schechter function to the corrected luminosity function to estimate galaxy distribution parameters.

![Luminosity Function](https://mjcowley.github.io/images/SDSS_Luminosity_Function.png)

## Usage

1. Clone this repository or download the Jupyter notebook.
2. Ensure that the required SDSS data is available or query it directly from the notebook.
3. Run the notebook to compute the luminosity function and fit the Schechter function.
4. Inspect the output CSV files for the fitted parameters and corrected luminosity function.

## Requirements

- Python 3.x
- `matplotlib`
- `pandas`
- `numpy`
- `astroquery`
- `scipy`
