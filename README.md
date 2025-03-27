# Code Repository for *Rodriguez et al. 2025*  

This repository provides several Jupyter notebooks to reproduce the source selection, photometry, and candidate selection processes from *Rodriguez et al. 2025*.  

## Available Notebooks  

- **Source Detection:**  
  - `Source_Detection_Find_Peaks.ipynb` → Identifies sources using Photutils find-peaks in the F335M JWST images.  

- **Photometry:**  
  - `PHANGS-JWST-Cycle1-Photometry.ipynb` → Performs aperture photometry on detected sources across HST and JWST bands.  

- **PAH Emitters Selection:**  
  - `PAH_Emitters_Selection.ipynb` → Identifies candidate 3.3µm PAH emitters.  

- **Color-Magnitude Diagram (CMD) for PAH Emitters Candidates:**  
  - `CMD_Selection.ipynb` → Generates the CMD for PAH emitter candidates (Fig. 2 in *Rodriguez et al. 2025*).  

- **Photometric Errors Plot:**  
  - `Phot-Error-Plot.ipynb` → Plots color errors (F300M - F335M) vs. F335M magnitude.  

## Data Sources  

The PHANGS-JWST and HST images can be found at:  
🔗 [PHANGS Archive](https://archive.stsci.edu/hlsp/phangs)  

## Complementary Data  

In the `ComplementaryData` folder, we provide several complementary files needed to run the code.  
For files required for each galaxy, we include an example for **NGC 7496**.  

### Foreground Extinction Tables for HST Filters  
- `foreground_exintion_new_filters.txt`  
- `phangs_hst_galactic_extinction_table.csv`  

### Vega Magnitude Zero Points for NGC 7496  
- `header_info_ngc7496_prime.txt`  

### PAH 3.3 Micron Emitters Selection for NGC 7496  
- **Between 3σ and 5σ color dispersion:** `population2_ngc7496.csv`  
- **Above 5σ color dispersion:** `population3_ngc7496.csv`  

### Color Dispersion Curve Parameters for NGC 7496  
- **3σ color dispersion curve parameters:** `Coef_dispersion_color_curve0_3sigma.csv`  
- **5σ color dispersion curve parameters:** `Coef_dispersion_color_curve0_5sigma.csv`  

### Detection Limits:  
- **F335M and F300M 5σ detection limits** (computed using randomly positioned apertures, as explained in *Rodriguez et al. 2025*):  
  - `Table_335_300_200_five_sigma.csv`  

