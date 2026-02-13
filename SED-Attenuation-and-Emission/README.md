# SED Attenuation and Emission Modelling

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="QARG" width="500" />

Python code for working with spectral energy distributions (SEDs), including:
- Applying Calzetti+ 2000 dust attenuation to an SED using a range of $A_V$ values.
- Adding dust emission to an SED using a blackbody emission model.

## Files

1. **S0_template_norm.sed** - Example SED template data file used for demonstration from [SWIRE Template Library](http://www.iasf-milano.inaf.it/~polletta/templates/swire_templates.html).
2. **S0_template_attenuated.sed** - Output file containing the attenuated SEDs for different $A_V$ values.

## Key Features

- **Plotting SEDs** - Visualise both the original and attenuated SEDs across different wavelength ranges.
- **Attenuation** - Apply the Calzetti+ (2000) attenuation law for various dust extinction values ($A_V$).
- **Dust Emission** - Add blackbody emission to simulate the impact of dust at a given temperature.
- **Output** - Save the attenuated SEDs to a file for further analysis.

![SED](https://mjcowley.github.io/images/SED-attenuation-and-emission.png)

## Requirements

- Python 3.x
- `matplotlib`
- `pandas`
- `numpy`