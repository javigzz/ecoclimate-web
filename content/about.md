---
title: "About ecoClimate"
date: 2020-01-11T01:54:45+01:00
---

The goal of ecoClimate is to provide an open database of processed climatic
simulations in a suitable resolution and user-friendly format for macroecological
and biogeographical studies. Our database includes all climate models currently
available from CMIP5 and PMIP3 projects for past, present, and future periods.

# Data availability

The dataset includes simulations for modern (1950-1999), historical (1900-1949), pre-industrial
(~1760), Mid-Holocene (6ka), Last Glacial Maximum (21ka), Pliocene (3Ma) and future conditions
(mean of simulations for 2080-2100), for nine coupled atmosphere-ocean global climate
models (AOGCMs). Future simulations include four representative concentration pathways
(RCPs): RCP2.6 (low emissions scenarios), RCP4.5 and RCP6.0 (intermediate emissions scenarios),
and RCP 8.5 (high emissions scenario) (see details in Taylor et al. 2009, 2012).

# Data downscaling

Monthly simulations of precipitation and mean, maximum and minimum temperature for all
time periods and AOGCMs were downloaded in netCDF format from [CMIP5](http://cmip-pcmdi.llnl.gov/cmip5/)
and [PMIP3](https://pmip3.lsce.ipsl.fr/), with spatial resolution originally ranging between 0.9o
(e.g., CCSM4) to 2.8o (e.g., MIROC-ESM).

All data were downscaled to 0.5o x 0.5o resolution, according to the standard change-factor
approach (Wilby et al. 2004), namely: i) firstly we computed the change-factor (also called
climate change trends or anomalies) between past/future and baseline climate for each raw variable
at model-specific native spatial resolution, (ii) secondarily we downscaled the change-factor
(instead of past/future climate values) and its respective baseline climate from each AOGCM to
the standard 0.5o resolution, and (iii) thirdly applied the downscaled change-factor to the
downscaled baseline climate to reconstitute values and obtain the downscaled layers for past
and future climates. From downscaled data, we generated the 19 bioclimatic variables described
in [WorldClim](http://www.worldclim.org/). This procedure was done using a script developed by
Matheus Lima-Ribeiro in https://github.com/ecoClimate.

# References

- TAYLOR KE, STOUFFER RJ and MEEHL GA (2009) A summary of the CMIP5 Experiment Design. Available
  in [CMIP5](http://cmip-pcmdi.llnl.gov/cmip5/).
- TAYLOR KE, STOUFFER RJ and MEEHL GA (2012) An overview of CMIP5 and the Experiment Design.
  American Meteorological Society. 93: 485–498.
- WILBY RL, CHARLES SP, ZORITA E, TIMBAL B, WHETTON P, MEARNS LO (2004) *Guidelines for use of
  climate scenarios developed from statistical downscaling methods*. IPCC Task Group on Data and
  Scenario Support for Impact and Climate Analysis. https://www.ipcc-data.org/guidelines/dgm_no2_v1_09_2004.pdf


# Acknowledgements

We first acknowledge the World Climate Research Programme’s Working Group on Coupled Modeling by the
[CMIP5](http://cmip-pcmdi.llnl.gov/cmip5/) and [PMIP3](https://pmip3.lsce.ipsl.fr/), and we thank the
climate modeling groups for producing and making available model outputs.

The U.S. Department of Energy’s Program for Climate Model Diagnosis and Intercomparison provides coordinating
support and led development of software infrastructure in partnership with the Global Organization for Earth
System Science Portals. We also thank Thiago F. Rangel (Universidade Federal de Goiás – Brazil) for help and
invaluable suggestions. The feedback from users who used our previous climatic data sets was also valuable.
Finally, we dedicate the ecoClimate to the memory of Mariana Rocha, who was enthusiastically interested in
this project when integrating the early ecoClimate team. We acknowledge financial support from CNPq, CAPES,
and FAPEG for supporting our work via multiple grants and fellowships, especially the research network
GENPAC (Geographical Genetics and Regional Planning for Natural Resources in Brazilian Cerrado).
