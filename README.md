
<!-- README.md is generated from README.Rmd. Please edit that file -->

# remice <a href = "https://erictong2.github.io/remice/"><img src="man/figures/logo.png" align="right" height="138"/></a>

Have your collaborators been remiss in their data collection? Have you
experienced characters in your numeric columns? Do rows ever get
incorrectly entered or swapped? Remice aims to provide a way to identify
and solve those problems.

The overarching goal of the remice package is to account for remiss
data.

## Installation

You can install the development version of remice like so:

``` r
#install_github("erictong2/remice")
```

## Function List

These are the functions included in the package:

- `analyze_type()` takes a column and determines if any values in that
  row are not of a specified type, which could cause errors for other
  functions

- `table_different()` creates a table of strings that are uncommonly
  found

- `separate_list()` creates a table of the most common responses, when
  multiple responses could exist in one row. For example, this could be
  used on a survey about comfort foods, where a response might be “”
  -plot_outliers uses longitunial data and checks for any abnormally
  large changes in the data. The user inputs a percent change, and any
  points above that will be plotted.

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(remice)
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.