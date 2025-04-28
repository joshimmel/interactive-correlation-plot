# An Interactive Correlation Plot for Oyster Creek Marshes 

This repository contains all the necessary ingredients for an interactive plotting and correlation tool that can test relationships between marsh sedimentation rates, in-situ, and environmental variables across sites.

The underlying data were generated from high-resolution sediment core analysis (MAR, SAR, LOI, DBD, grain size distributions) collected from a transect of cores on a marsh platform in Oyster Creek, NC ( OC-21-01 at 2 meters from edge in 2021, OC-21-02 at 8 meters from edge in 2021, OC-21-03 at 15 meters from edge in 2021). Annualized site-specific variables were interpolated from centimeter-scale core measurements using PCHIP interpolation to produce continuous year-by-year datasets for cross-correlation.

In addition, broader site-agnostic variables (e.g., mean sea level, land cover classifications, relative distances across the marsh platform) were compiled and interpolated separately (linear interpolation).

## Variables

- **MAR** — Mass Accumulation Rate (g/cm²/yr)
- **SAR** — Sediment Accumulation Rate (cm/yr)
- **LOI** — Loss on Ignition (fractional mass, g/g)
- **DBD** — Dry Bulk Density (g/cm³)
- **d5, d50, d95** — Grain size percentiles (µm)

Additional variables (e.g., mean sea level, land cover categories, inundation fraction) represent broader marsh-scale or environmental factors.

## Purpose

This tool enables users to:
- Select two sites (or "site-agnostic" for environmental variables)
- Select a variable from each site (e.g., MAR vs. LOI)
- Specify a year range for comparison
- Visualize full and zoomed-in trends over time
- Calculate and display Pearson and Spearman correlation coefficients dynamically for the selected year range

The tool is intended to facilitate exploratory comparisons of sediment accumulation rates (and related core-derived metrics) against environmental drivers across space and time.

## Usage

Launch the app via Voilà to use the dropdown selectors and interactive plots.  
The figure dynamically updates based on the selected sites, variables, and time window, making it easier to test hypotheses about sedimentation-environment relationships across the marsh platform.

[![Launch Voilà](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/joshimmel/interactive-correlation-plot/HEAD?urlpath=voila/render/interactive_correlation_plot.ipynb)
