# Byrd Glacier: Geostatistical Markov Chain Monte Carlo (MCMC) Analysis

## Description
Bed topography mapping of **Byrd Glacier** using Sequential Gaussian Simulation (SGS) and a Markov Chain Monte Carlo (MCMC) framework, built on top of BedMachine/Bedmap3 products and compiled radar thickness measurements. This repository walks through the full workflow from loading and cleaning Antarctic datasets, constructing a 500 m grid of surface, thickness, and bed, and defining a fast-flowing grounded-ice mask, to fitting a Matern variogram, running SGS to generate geostatistical bed realizations, and using mass-conservation flux divergence to evaluate each realization. By treating bed elevation as a random field and sampling it in a Bayesian framework, the project focuses on how uncertainty in subglacial topography propagates into mass conservation residuals and where Byrd Glacier’s flux budget is most sensitive to bed errors. All code used for labs, variogram analysis, SGS simulations, residual calculations, and final poster figures is collected here for reproducibility and future extension.

---

## Figures

**A) Surface Ice Velocity Magnitude**  
Large-scale view of surface speed over the Byrd Glacier catchment, used to define fast-flowing regions and flux gates.

**B) Radar Data Coverage**  
Map of radar bed picks indicating where we have direct thickness constraints and where the model must interpolate.

**C) Region Mask + Grounding Line**  
Binary mask for the Byrd domain plus grounding line geometry used to define the model boundaries.

**D) BedMachine Bed Elevation**  
Existing bed product used as a reference surface and baseline for flux divergence and thickness comparisons.

**E) BedMap3 Bed Elevation**  
Alternate large-scale bed product for the same domain, highlighting differences in trough structure and sill heights.

**F) Geostatistical Realization**  
An SGS-based bed realization at 500 m resolution that honors radar data and spatial covariance, used as an initial condition for MCMC.

**G) Velocity with Lat & Lon**  
Surface velocity plotted in geographic coordinates (lat/lon) for easier comparison with external datasets and published maps.

**H) Antarctica With Study Area**  
Locator map showing the position of Byrd Glacier within the larger Antarctic ice sheet.

**I) Surface Elevation Change Rate**  
dh/dt field used as a soft constraint in the mass conservation equation for the MCMC workflow.

**J) Histogram of Mass Conservation Residual**  
Distribution of flux divergence residuals, used to evaluate how well a given bed realization satisfies mass conservation.

**K) Isotropic Experimental Variogram**  
Empirical variogram of the normal-score bed data, used to set variogram parameters for SGS and to inform prior structure in MCMC.

**Final Realizations**

---

# Installation

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Basic Python environment with `numpy`, `pandas`, and geostatistics tools is assumed.

---

# Tutorial

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Placeholder for a short step-by-step example running SGS, computing residuals, and plotting one chain from the MCMC.

---

## Poster
Final Poster
[annotated-GLY4930%20Poster%20-%20Byrd%20Glacier%20-%20Kalim%20Qazi.pdf](https://github.com/user-attachments/files/23615942/annotated-GLY4930.20Poster.20-.20Byrd.20Glacier.20-.20Kalim.20Qazi.pdf)
