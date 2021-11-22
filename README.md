
# The VDDG model forced by the Jin-Timmermann ENSO model 

[![DOI](https://zenodo.org/badge/360905794.svg)](https://zenodo.org/badge/latestdoi/360905794)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## General Information

These Jupyter notebooks come as a supplementary material to the article :

* Vannitsem, S., Demaeyer, J., and Ghil, M. (2021). Extratropical low‐frequency variability with ENSO forcing: A reduced‐order coupled model study. *Journal of Advances in Modeling Earth Systems*, e2021MS002530. [https://doi.org/10.1029/2021MS002530](https://doi.org/10.1029/2021MS002530).

and detail the computations performed to obtain the results therein.

These notebooks contains the model VDDG forced by the Jin-Timmermann model for ENSO variability. The VDDG model is obtained through [qgs](https://github.com/Climdyn/qgs) configured to run the coupled ocean-atmosphere [MAOOAM](https://github.com/Climdyn/MAOOAM) model.

More details are available inside the notebooks:

* [vddg_enso.ipynb](./vddg_enso.ipynb): contains the forced model and integrate it to get several trajectories.
* [vddg_enso_lyapunov.ipynb](./vddg_enso_lyapunov.ipynb): in this notebook the forced model is integrated to get several trajectories, and their first Lyapunov exponent is computed.

## About

Copyright (c) 2021 Jonathan Demaeyer

See [LICENSE.txt](./LICENSE.txt) for license information.

## Requirements

The present notebooks were tested on a computer with

    12 recent cpu cores,
    16 Gb of RAM,

## Installation

To install these notebooks, you must first [install the qgs model](https://qgs.readthedocs.io/en/latest/files/general_information.html#installation) and test that it works properly on your machine. Follow the instructions in the model documentation. Then you must move the notebooks in the notebooks directory and run it with jupyter-notebook. In the qgs model main folder, do:

    conda activate qgs
    cd notebooks
    jupyter-notebook

It will open a page in a web browser where you can open and then run the notebooks.

