# Solar Elevation Calculator – Kidney Lawn Edition

<img src="https://mjcowley.github.io/images/qarg_bw.png" alt="Sun diagram" width="420"/>

Interactive Jupyter notebook that generates half‑hour solar‑elevation tables for any date and location.  
Originally built for QUT’s *AstroLab E1 – Solar Shadows and Solar Time* activity.

## What It Does

* Prompts for **Latitude**, **Longitude** and **Date** via notebook widgets.  
* Computes Sun altitude (`AltAz`) at 30‑minute steps (09 h – 15 h local).  
* Prints a clean table ready to paste into lab hand‑outs.  
* Uses **Astropy** for precise solar positions.

## Repository Contents

| File | Purpose |
|------|---------|
| `Solar Calculator.ipynb` | Main interactive notebook with widgets and calculation code. |
| `requirements.txt` | Minimal package list to recreate the environment. |
| `LICENSE` | MIT License. |

## Quick Start

```bash
# Clone and enter the project
git clone https://github.com/YOUR_USERNAME/solar-elevation-calculator.git
cd solar-elevation-calculator

# Create environment (conda example)
conda env create -f environment.yml
conda activate solar-sun

# Or: pip install
pip install -r requirements.txt

# Launch Jupyter
jupyter lab Solar\ Calculator.ipynb
```

1. Enter your site coordinates and desired date.  
2. Run the calculation cell.  
3. Copy the printed table into your LaTeX hand‑out.

## Dependencies

* Python 3.10 +
* `astropy`
* `pandas`
* `numpy`
* `pytz`
* `ipywidgets`

Install via `requirements.txt` or create a conda environment.

## Example Output

```
Solar Elevation for (‑27.4771, 153.0293)
Date: 04 August 2025
--------------------------------------
Time (AEST)  Elevation (°)
09:00        27.3
09:30        32.1
...
15:00        27.5
```

## Citation

If you use this notebook in published work, please cite:

> Cowley, M. J. (2025). *AstroLab E1: Solar Shadows and Solar Time*.

## License

Licensed under the MIT License – see the `LICENSE` file for details.
