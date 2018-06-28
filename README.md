
<!-- README.md is generated from README.Rmd. Please edit that file -->

# <img src="https://i.imgur.com/vTLlhbp.png" align="right" height=88 /> Open datasets of ForestGEO

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/fgeo.data)](https://cran.r-project.org/package=fgeo.data)
[![Travis build
status](https://travis-ci.org/forestgeo/fgeo.data.svg?branch=master)](https://travis-ci.org/forestgeo/fgeo.data)

## Installation

[Install all **fgeo** packages in one
step](https://forestgeo.github.io/fgeo/index.html#installation)

    # install.packages("remotes")
    remotes::install_github("forestgeo/fgeo.data")

For details on how to install packages from GitHub, see [this
article](https://goo.gl/dQKEeg).

## Example

``` r
library(fgeo.data)

# Show first few columns to save space.
str(luquillo_vft_4quad, give.attr = FALSE, list.len = 5)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    3302 obs. of  32 variables:
#>  $ DBHID           : int  384550 384553 466764 384554 466765 611446 384555 466766 611447 384556 ...
#>  $ PlotName        : chr  "luquillo" "luquillo" "luquillo" "luquillo" ...
#>  $ PlotID          : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ Family          : chr  "Rubiaceae" "Urticaceae" "Urticaceae" "Urticaceae" ...
#>  $ Genus           : chr  "Psychotria" "Cecropia" "Cecropia" "Cecropia" ...
#>   [list output truncated]

# See ?data_dictionary
```

[Get started with
**fgeo**](https://forestgeo.github.io/fgeo/articles/fgeo.html)

## Information

  - [Getting help](SUPPORT.md).
  - [Contributing](CONTRIBUTING.md).
  - [Contributor Code of Conduct](CODE_OF_CONDUCT.md).

## Acknowledgements

  - Thanks to Suzanne Lao and Shameema Jafferjee Esufali for sharing
    their knowledge of the structure of ForestGEO’s database.

  - Thanks to Jess Zimmerman for sharing data from Luquillo.
