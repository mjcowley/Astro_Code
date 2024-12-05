# SED Attenuation and Emission Modelling

![QARG](https://mjcowley.github.io/images/qarg_bw.png)

Python code for working with spectral energy distributions (SEDs), including:
- Applying Calzetti+ 2000 dust attenuation to an SED using a range of $A_V$ values.
- Adding dust emission to an SED using a blackbody emission model.

## Files

1. **S0_template_norm.sed**: Example SED template data file used for demonstration from [SWIRE Template Library](http://www.iasf-milano.inaf.it/~polletta/templates/swire_templates.html).
2. **S0_template_attenuated.sed**: Output file containing the attenuated SEDs for different $A_V$ values.

## Key Features

- **Plotting SEDs**: Visualise both the original and attenuated SEDs across different wavelength ranges.
- **Attenuation**: Apply the Calzetti+ (2000) attenuation law for various dust extinction values ($A_V$).
- **Dust Emission**: Add blackbody emission to simulate the impact of dust at a given temperature.
- **Output**: Save the attenuated SEDs to a file for further analysis.

## Usage

1. Clone this repository or download the Jupyter notebook.
2. Ensure the S0_template_norm.sed file is available in your directory.
3. Run the Python code to plot and output the attenuated SEDs for various $A_V$ values.
