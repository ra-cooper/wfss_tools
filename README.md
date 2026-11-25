# Update 25/11/26

New example notebooks have been added. These are much more streamlined and make better use of grizli's built-in routines.


# Example notebooks for working with NIRCam WFSS Data

Some example notebooks for working with JWST NIRCam WFSS data. The three notebooks are designed to work together and follow the same file structure. The extraction procedure uses grizli as its core, details of which can be found [here](https://github.com/gbrammer/grizli)

## Notebook 00_wfss_data_reduction.ipynb

Notebook for reducing NIRCam WFSS data. Performs background subtraction and continuum subtraction with emission line masking. The notebook automatically detects filters and GRISMS and adjusts the reduction procedure accordingly. This notebook can be used if you intend on extracting spectra manually (without grizli)

## Notebook 01_prep_wfss_data.ipynb

Notebook demonstration on using grizli to initiate WFSS imaging and produce contamination models from a segmentation map and direct imaging.


## Notebook 02_extraction_stacking.ipynb

Should be run after Notebook 01. Performs the extraction and stacking for objects in a target catalogue.



