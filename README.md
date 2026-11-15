# Example notebooks for working with NIRCam WFSS Data

Some example notebooks for working with JWST NIRCam WFSS data. The three notebooks are designed to work together and follow the same file structure. The extraction procedure uses grizli as its core, details of which can be found [here](https://github.com/gbrammer/grizli)

## 0.0 wfss_data_reduction.ipynb

Notebook for reducing NIRCam WFSS data. Performs background subtraction and continuum subtraction with emission line masking. The notebook automatically detects filters and GRISMS and adjusts the reduction procedure accordingly.

## 1.0 wfss_initialisation.ipynb

Notebook utilising grizli to initialise and build footprints. Requires both GRISM and direct images of matching filters.


## 2.0 wfss_extraction.ipynb

Notebook utilising grizli to extract spectra for a given list of coordinates. This notebook can perform extraction across multiple filters, grisms, and dispersion directions. Outputs include stacked 2D spectra and visualisations.
**Note:** If you want to use files produced by notebook 0, you must remove the contamination modelling from this notebook.

