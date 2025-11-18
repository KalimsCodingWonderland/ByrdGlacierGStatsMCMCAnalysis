# ByrdGlacierGStatsMCMCAnalysis

## Description
Bed topography mapping of **Byrd Glacier** using Sequential Gaussian Simulation (SGS) and a Metropolis–Hastings (MCMC) framework, with a focus on how bed uncertainty propagates into mass conservation residuals.

## Note
Figures are saved as `.svg` where possible. For best quality, download and view locally rather than relying on the GitHub preview.

---

## Initial Topographies

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

---

## MCMC Topography

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

---

# Installation

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Basic Python environment with `numpy`, `pandas`, and geostatistics tools is assumed.

---

# Tutorial

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Placeholder for a short step-by-step example running SGS, computing residuals, and plotting one chain from the MCMC.

---

## Poster

Final Poster
