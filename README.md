
<!-- README.md is generated from README.Rmd. Please edit that file -->

# <img src="https://i.imgur.com/39pvr4n.png" align="right" height=44 /> fgeo.opendata

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/fgeo.opendata)](https://cran.r-project.org/package=fgeo.opendata)
[![Travis build
status](https://travis-ci.org/forestgeo/fgeo.opendata.svg?branch=master)](https://travis-ci.org/forestgeo/fgeo.opendata)

The goal of **fgeo.opendata** provides open datasets of ForestGEO.

## Installation

    # install.packages("remotes")
    remotes::install_github("forestgeo/fgeo.opendata")

For details on how to install packages from GitHub, see [this
article](https://goo.gl/dQKEeg).

## Example

``` r
library(fgeo.opendata)

# Details: https://forestgeo.github.io/fgeo.opendata/reference/taxa_bci
str(taxa_bci, give.attr = FALSE)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    1428 obs. of  21 variables:
#>  $ ViewID        : int  1 2 3 4 5 6 7 8 9 10 ...
#>  $ SpeciesID     : int  1 3 4 5 6 7 8 9 10 11 ...
#>  $ SubspeciesID  : chr  NA NA NA NA ...
#>  $ Family        : chr  "Fabaceae-mimosoideae" "Fabaceae-mimosoideae" "Fabaceae-mimosoideae" "Fabaceae-mimosoideae" ...
#>  $ Mnemonic      : chr  "pit1ba" "acacco" "acacme" "acac1" ...
#>  $ Genus         : chr  "Abarema" "Acacia" "Acacia" "Acacia" ...
#>  $ SpeciesName   : chr  "barbouriana" "collinsii" "melanoceras" "sp.1" ...
#>  $ Rank          : chr  NA NA NA NA ...
#>  $ Subspecies    : chr  NA NA NA NA ...
#>  $ Authority     : chr  "(Standl.) Barneby & J.W. Grimes" "Saff." "Beurl." NA ...
#>  $ IDLevel       : chr  "species" "species" "species" "genus" ...
#>  $ subspMnemonic : chr  NA NA NA NA ...
#>  $ subspAuthority: chr  NA NA NA NA ...
#>  $ FieldFamily   : chr  NA NA NA NA ...
#>  $ Lifeform      : chr  NA NA NA NA ...
#>  $ Description   : chr  NA NA NA NA ...
#>  $ wsg           : num  0.567 0.775 0.775 0.775 0.3 ...
#>  $ wsglevel      : chr  "genus" "genus" "genus" "genus" ...
#>  $ ListOfOldNames: chr  NA NA NA NA ...
#>  $ Specimens     : chr  NA NA NA NA ...
#>  $ Reference     : chr  NA NA NA NA ...

# Details: https://forestgeo.github.io/fgeo.opendata/reference/vft_random_bci
str(vft_random_bci, give.attr = FALSE)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    2257 obs. of  32 variables:
#>  $ DBHID           : int  1621522 1619521 1632477 1630644 1077531 1074697 826469 823306 1006845 1003843 ...
#>  $ PlotName        : chr  "bci" "bci" "bci" "bci" ...
#>  $ PlotID          : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ Family          : chr  "Violaceae" "Violaceae" "Fabaceae-papilionoideae" "Fabaceae-papilionoideae" ...
#>  $ Genus           : chr  "Hybanthus" "Hybanthus" "Lonchocarpus" "Lonchocarpus" ...
#>  $ SpeciesName     : chr  "prunifolius" "prunifolius" "heptaphyllus" "heptaphyllus" ...
#>  $ Mnemonic        : chr  "hybapr" "hybapr" "loncla" "loncla" ...
#>  $ Subspecies      : chr  NA NA NA NA ...
#>  $ SpeciesID       : int  494 494 1134 1134 99 99 895 895 980 980 ...
#>  $ SubspeciesID    : chr  NA NA NA NA ...
#>  $ QuadratName     : chr  "4715" "4715" "0022" "0022" ...
#>  $ QuadratID       : int  3012 3012 1261 1261 2241 2241 3052 3052 2315 2315 ...
#>  $ PX              : num  957.3 957.3 16.3 16.3 324.6 ...
#>  $ PY              : num  307 307 442 442 392 ...
#>  $ QX              : num  17.3 17.3 16.3 16.3 4.6 4.6 0.3 0.3 0.6 0.6 ...
#>  $ QY              : num  6.9 6.9 2.5 2.5 12.4 12.4 18.2 18.2 1 1 ...
#>  $ TreeID          : int  267125 267125 269374 269374 159260 159260 109920 109920 145725 145725 ...
#>  $ Tag             : chr  "312412" "312412" "400860" "400860" ...
#>  $ StemID          : int  267125 267125 577077 577077 159260 159260 109920 109920 145725 145725 ...
#>  $ StemNumber      : int  1 1 2 2 1 1 1 1 1 1 ...
#>  $ StemTag         : int  NA NA NA NA NA NA NA NA NA NA ...
#>  $ PrimaryStem     : chr  "main" "main" "main" "main" ...
#>  $ CensusID        : int  6 171 6 171 6 171 6 171 6 171 ...
#>  $ PlotCensusNumber: int  6 7 6 7 6 7 6 7 6 7 ...
#>  $ DBH             : num  27 30 NA NA 42 NA 26 28 28 40 ...
#>  $ HOM             : num  1.3 1.3 NA NA 1.3 NA 1.3 1.3 1.3 1.3 ...
#>  $ ExactDate       : Date, format: "2005-10-05" "2010-09-06" ...
#>  $ Date            : int  16714 18511 16492 18323 16544 18378 16702 18507 16572 18395 ...
#>  $ ListOfTSM       : chr  NA NA "OR" "D;N" ...
#>  $ HighHOM         : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ LargeStem       : chr  NA NA NA NA ...
#>  $ Status          : chr  "alive" "alive" "broken below" "dead" ...

# Details: https://forestgeo.github.io/fgeo.opendata/reference/vft_1ha_bci
# Similar to `vft_random_bci`; truncating list output for space
str(vft_1ha_bci, give.attr = FALSE, list.len = 5)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    10543 obs. of  32 variables:
#>  $ DBHID           : int  148842 150985 148877 148912 151013 149016 151095 149050 151122 149083 ...
#>  $ PlotName        : chr  "bci" "bci" "bci" "bci" ...
#>  $ PlotID          : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ Family          : chr  "Simaroubaceae" "Simaroubaceae" "Sapotaceae" "Sapotaceae" ...
#>  $ Genus           : chr  "Simarouba" "Simarouba" "Pouteria" "Pouteria" ...
#>   [list output truncated]

# Details: https://forestgeo.github.io/fgeo.opendata/reference/census_bci
str(tree6_random_bci, give.attr = FALSE)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    1000 obs. of  16 variables:
#>  $ treeID   : num  590 1057 1451 2362 2867 ...
#>  $ tag      : chr  "000580" "001054" "001449" "002369" ...
#>  $ sp       : chr  "virosp" "alsebl" "quaras" "quaras" ...
#>  $ quadrat  : chr  "4614" "4317" "4113" "3618" ...
#>  $ gx       : num  933 866 831 737 669 ...
#>  $ gy       : num  283 358 277 371 194 ...
#>  $ stemID   : int  590 1057 1451 2362 2867 2912 3477 3492 3707 4822 ...
#>  $ dbh      : num  330 344 857 640 411 371 233 823 238 585 ...
#>  $ hom      : num  1.3 3 4 5.85 3 3.6 3.7 1.3 1.3 4 ...
#>  $ ExactDate: chr  "2005-09-19" "2005-10-12" "2005-10-11" "2005-10-11" ...
#>  $ codes    : chr  NA "B;cylN" "B;cylN" "B;cylN" ...
#>  $ date     : num  16698 16721 16720 16720 16711 ...
#>  $ status   : chr  "A" "A" "A" "A" ...
#>  $ nostems  : int  1 1 1 1 1 1 1 1 1 1 ...
#>  $ agb      : num  0.706 0.919 7.294 3.654 1.414 ...
#>  $ ba       : num  0.0855 0.0929 0.5768 0.3217 0.1327 ...

# Details: https://forestgeo.github.io/fgeo.opendata/reference/census_bci
str(stem7_1ha_bci, give.attr = FALSE)
#> Classes 'tbl_df', 'tbl' and 'data.frame':    10373 obs. of  16 variables:
#>  $ treeID   : num  1853 1857 1861 1864 1866 ...
#>  $ stemID   : num  1853 1857 1861 1864 1866 ...
#>  $ tag      : chr  "001854" "001858" "001862" "001865" ...
#>  $ StemTag  : chr  "" "" "" "" ...
#>  $ sp       : chr  "simaam" "poutre" "quaras" "guargr" ...
#>  $ quadrat  : chr  "3909" "3909" "3908" "3908" ...
#>  $ gx       : num  792 793 783 799 793 ...
#>  $ gy       : num  181 190 177 168 170 ...
#>  $ dbh      : num  555 455 778 304 454 595 229 500 335 560 ...
#>  $ hom      : num  1.3 3.7 6 1.3 3.75 6.8 3 3.8 1.3 3 ...
#>  $ ExactDate: chr  "2010-07-27" "2010-09-07" "2010-09-10" "2010-07-23" ...
#>  $ DFstatus : chr  "alive" "alive" "alive" "alive" ...
#>  $ codes    : chr  NA "B;cylN" "B;cylN" NA ...
#>  $ date     : num  18470 18512 18515 18466 18512 ...
#>  $ status   : chr  "A" "A" "A" "A" ...
#>  $ agb      : num  2.189 2.763 5.819 0.681 2.336 ...

# Details: https://forestgeo.github.io/fgeo.opendata/reference/elevation_bci
str(elevation_bci)
#> List of 4
#>  $ col :'data.frame':    20301 obs. of  3 variables:
#>   ..$ x   : int [1:20301] 0 0 0 0 0 0 0 0 0 0 ...
#>   ..$ y   : int [1:20301] 0 5 10 15 20 25 30 35 40 45 ...
#>   ..$ elev: num [1:20301] 121 121 121 121 121 ...
#>  $ mat : num [1:101, 1:201] 121 121 121 121 121 ...
#>  $ xdim: int 1000
#>  $ ydim: int 500
```

## Raw data (database output)

  - The raw data (database output) on which this data-package is based
    can be downloaded directly from <http://bit.ly/database-output>.
    This is useful for examples using the data exactly as it is
    delivered from the database to the users – particularly for examples
    of reading .csv files and data cleaning. You can also download
    specific files, as follows. To find links to download each raw
    dataset individually see the help file of each
dataset.

<!-- end list -->

``` r
# IMPORTANT if reading raw data (e.g. .csv files from ForestGEO's database)

# Raw data (normally you would have a .csv file stored in your computer)
url <- "http://bit.ly/fgeo-opendata-taxa-bci"

# TO AVOID ERRORS
# Specify columns class explicitely (for an example showing only some columns)
column_classes <- c(
  ViewID = "integer", 
  SpeciesID = "integer", 
  SubspeciesID = "integer", 
  Family = "character", 
  Mnemonic = "character"
)
# Specify how to interprate missing values
na_strings <- c("", "NA", "NULL")

raw_taxa_bci <- read.delim(
  file = url, 
  na.strings = na_strings, 
  colClasses = column_classes
)

some_rows <- some_columns <- 1:5
raw_taxa_bci[some_rows, some_columns]
#>   ViewID SpeciesID SubspeciesID               Family Mnemonic
#> 1      1         1           NA Fabaceae-mimosoideae   pit1ba
#> 2      2         3           NA Fabaceae-mimosoideae   acacco
#> 3      3         4           NA Fabaceae-mimosoideae   acacme
#> 4      4         5           NA Fabaceae-mimosoideae    acac1
#> 5      5         6           NA        Euphorbiaceae   acaldi

# Note these are the same as `column_classes` defined above
sapply(raw_taxa_bci[some_rows, some_columns], class)
#>       ViewID    SpeciesID SubspeciesID       Family     Mnemonic 
#>    "integer"    "integer"    "integer"  "character"  "character"
```

## Code of Conduct

Please note that this project is released with a [Contributor Code of
Conduct](.github/CODE_OF_CONDUCT.md). By participating in this project
you agree to abide by its terms.
