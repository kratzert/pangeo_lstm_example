# Rainfall-runoff modelling using LSTMs

[![Binder](https://binder.pangeo.io/badge_logo.svg)](https://binder.pangeo.io/v2/gh/kratzert/pangeo_lstm_example/master)

This is an example notebook on how to use LSTMs for rainfall-runoff simulations. We make use of the [PyTorch](https://pytorch.org/) deep learning library and the [CAMELS](https://ral.ucar.edu/solutions/products/camels) data set

## Run on Pangeo cluster
Click the `launch binder` button/icon above to run the notebook on the [Pangeo](https://pangeo.io/) server and to walk through this example without the need of installing anything.

## Run locally

1. Download the CAMELS data set from [here](https://ral.ucar.edu/solutions/products/camels)

2. Download and extract or clone the `run_local` branch `git clone -b run_local --single-branch git@github.com:kratzert/pangeo_lstm_example.git`

3. (Optionally) Create conda environment from the `environment.yml` file in the `binder/` directory. If you have a GPU available, make sure to install the PyTorch GPU version.

4. Start Jupyter Notebook/Lab and make sure to change the `CAMELS_PATH` in the first code box to your local CAMELS path.

## Related article
In our paper ["Rainfall–runoff modelling using Long Short-Term Memory (LSTM) networks"](https://www.hydrol-earth-syst-sci.net/22/6005/2018/) we tested the LSTM on various basins of the CAMELS data set. This notebook shows how to replicate experiment 1 of the paper in which one LSTM is trained per basin. Note: This is not an exact replication of the model setup, but can be easily extended to the settings of the paper.

If you use this repository in your work, please cite:
```
Kratzert, F., Klotz, D., Brenner, C., Schulz, K., and Herrnegger, M.: Rainfall–runoff modelling using Long Short-Term Memory (LSTM) networks, Hydrol. Earth Syst. Sci., 22, 6005-6022, https://doi.org/10.5194/hess-22-6005-2018, 2018. 
```