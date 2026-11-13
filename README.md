# Astro_Code

<img src="Images/qarg_bw_dark.png" alt="QUT Logo" width="500" />

Welcome to the QUT Astrophysics Research Group [(QARG)](https://research.qut.edu.au/qutastrophysics/) repository, a collection of Python code for various astronomical analyses. This repository includes tools and scripts for tasks such as data analysis, modelling, visualisation, and fitting in astronomy.

## Notebooks

Each folder is self-contained, with its own README describing the notebook in more detail.

| Folder | Description | Data source |
|---|---|---|
| [SDSS-Luminosity-Function](SDSS-Luminosity-Function) | Builds the r-band galaxy luminosity function with the 1/Vmax method and fits a Schechter function | SDSS DR18 (queried live) |
| [SED-Attenuation-and-Emission](SED-Attenuation-and-Emission) | Applies Calzetti (2000) dust attenuation and blackbody dust emission to a galaxy SED template | Included SWIRE template |
| [Solar-Calculator](Solar-Calculator) | Interactive table of solar elevation through the day for any location and date | Computed with Astropy |
| [ZFOURGE-VizieR-Import](ZFOURGE-VizieR-Import) | Retrieves ZFOURGE catalogues from VizieR, applies the `use` flag, and plots stellar mass against redshift | ZFOURGE via VizieR |
| [ZFOURGE-RestFrame-UVJ](ZFOURGE-RestFrame-UVJ) | Rest-frame UVJ diagram for COSMOS galaxies, coloured by specific star formation rate | ZFOURGE via VizieR |
| [ZFOURGE-EAZY](ZFOURGE-EAZY) | Full eazy-py pipeline: photometric redshifts, stellar population properties, and an interactive explorer | ZFOURGE via VizieR |

## Getting Started

Install the dependencies for all notebooks except ZFOURGE-EAZY:

```bash
pip install -r requirements.txt
```

ZFOURGE-EAZY has heavier dependencies, listed in [ZFOURGE-EAZY/requirements.txt](ZFOURGE-EAZY/requirements.txt). Its first cell also installs anything missing.

Then open a notebook with Jupyter, from inside its folder so it can find its data files:

```bash
jupyter lab
```

Notebooks that query VizieR save a copy of each catalogue in a local `vizier_cache` folder, so later runs work without downloading again.

## Contributing

Contributions are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.

## Acknowledgements

Special thanks to all contributors and to the open-source communities that make scientific computing and data analysis possible.
