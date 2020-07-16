
<!-- README.md is generated from README.Rmd. Please edit that file -->

# UNSEEN

<!-- badges: start -->

<!-- badges: end -->

The goal of UNSEEN is to provide easy evaluation of the UNSEEN method,
developed for the SEAS5 hindcast data during the ECMWF Summer of Weather
Code ([ESoWC 2020](https://github.com/esowc/UNSEEN-open)).

## Installation

<!-- You can install the released version of UNSEEN from [CRAN](https://CRAN.R-project.org) with: -->

<!-- ``` r -->

<!-- install.packages("UNSEEN") -->

<!-- ``` -->

You can install the development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("timokelder/UNSEEN")
```

## Example

This is a basic example which shows you how to plot the UNSEEN
timeseries, using the example dataset:

``` r
data("EOBS_UK","SEAS5_UK")
```

``` r
library(UNSEEN)
## basic example code

unseen_timeseries(ensemble = SEAS5_UK, obs = EOBS_UK, ylab = 'UK February precipitation (mm/d)')
```

<img src="man/figures/README-example-1.png" width="100%" />