# 2020-ncov

Analysis of the 2020 nCoV outbreak. _Note: this is working repository, so code and data are likely to change over time_

### Guide to files for `stoch_model`

This is a stochastic SEIR model implemented using Euler-Maruyama, with likelihood estimated using SMC by fitting to exported cases over time in countries with high connectivity to Wuhan.

Data loading and model run script is in `scripts/main_model.r`. Calls the following files:

> `R/load_timeseries.r` - Load and format timeseries

> `R/model_functions.r` - Load process model and SMC

> `R/plotting_functions.r` - Plotting