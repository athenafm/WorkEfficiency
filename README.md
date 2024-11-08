
<!-- README.md is generated from README.Rmd. Please edit that file -->

# WorkEfficiency

<!-- badges: start -->
<!-- badges: end -->

The goal of WorkEfficiency is to create a simple and easy way to calculate the total work efficiency during a Metabolic visit at McMaster University. This package will take values from the Total Energy Expended and Resting Energy Expenditure to give a value that corresponds with work efficiency. Both of these values can be obtained experimentally through indirect calorimetry. You can find the corresponding sample data sets in the data folder that you can practice with. You can also find some test runs in the folder test that validates the formula and packages to ensure it is working properly. Lastly, in the man folder you can find the documentation related to this package.


## Installation
```r
install.packages("devtools")
install.packages("usethis")
library(devtools)
library(usethis)
install_github("athenafm/WorkEfficiency")
library(WorkEfficiency)
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(WorkEfficiency)
calculate_work_efficiency(1500,2000)
[1] 0.25 
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
