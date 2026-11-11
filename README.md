# Example notebooks for working with NIRCam WFSS Data

Some example notebooks for working with JWST data. The three notebooks are designed to work together and follow the same file structure. The extraction procedure uses grizli as its core, details of which can be found [here](https://github.com/gbrammer/grizli)

## 1. wfss_data_reduction.ipynb

Notebook for reducing NIRCam WFSS data. Performs background subtraction and continuum subtraction with emission line masking. The notebook automatically detects filters and GRISMS and adjusts the reduction procedure accordingly.

## 2. wfss_initialisation.ipynb

Notebook utilising grizli to initialise and build footprints. Requires both GRISM and direct images of matching filters.
**Note:** Since data are already background subtracted and continuum subtracted, these steps are skipped in the overall grizli pipeline.

## 3. wfss_extraction.ipynb

Notebook utilising grizli to extract spectra for a given list of coordinates. This notebook can perform extraction across multiple filters, grisms, and dispersion directions. Outputs include stacked 2D spectra and visualisations.
