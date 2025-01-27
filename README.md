
<!-- README.md is generated from README.Rmd. Please edit that file -->

# outils

<!-- badges: start -->
<!-- badges: end -->

The goal of outils is to define some utilities that could help in usual
R working.

## Installation

You can install the development version of outils like so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
```

## Example

``` r
library(outils)

get_working_files()
#> [1] "dev/0-dev_history.Rmd"                   
#> [2] "dev/flat_outils.Rmd"                     
#> [3] "R/get_function_names.R"                  
#> [4] "R/get_working_files.R"                   
#> [5] "README.Rmd"                              
#> [6] "tests/testthat.R"                        
#> [7] "tests/testthat/test-get_function_names.R"
#> [8] "tests/testthat/test-get_working_files.R" 
#> [9] "vignettes/outils.Rmd"

working_files <- get_working_files()
if (length(working_files) > 1) {
  get_function_names(get_working_files()[[2]])
}
#> [1] "get_working_files"  "get_function_names"
```
