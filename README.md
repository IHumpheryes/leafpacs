
<!-- README.md is generated from README.Rmd. Please edit that file -->

# LEAFPACS <img src='https://github.com/aquaMetrics/leafpacs/raw/main/inst/extdat/images/leafpacs_logo.png' align="right" height="300" />

<!-- badges: start -->
<!-- badges: end -->

THIS PACKAGE IS A WORK IN PROGRESS PLEASE DON’T USE IN PRODUCTION.

The goal of `leafpacs` R package is to calculate river LEAFPACS
classification.

## Installation

Install the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("aquaMetrics/leafpacs")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(leafpacs)
## basic example
data <- leafpacs(get_demo_data())
#> Validating data
#> Loading demo data
#> Calculating indices
#> Calculating class
#> THIS PACKAGE IS A WORK IN PROGRESS PLEASE DON'T USE IN PRODUCTION.
#> Calculating confidence
#> All done!
head(data[, c("SAMPLE_ID", "CLASS", "RMHI")])
#>   SAMPLE_ID    CLASS RMHI
#> 1    662443 MODERATE 7.87
#> 2    741954 MODERATE 8.05
#> 3    672991 MODERATE 8.36
#> 4    742316 MODERATE 8.33
#> 5    373018     GOOD 7.95
#> 6    373017     GOOD 7.87
```
