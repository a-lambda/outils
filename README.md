
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

get_function_names(get_working_files())
#>                                     fichier           fonction
#> 1                     dev/0-dev_history.Rmd               <NA>
#> 2                       dev/flat_outils.Rmd  get_working_files
#> 3                       dev/flat_outils.Rmd get_function_names
#> 4                    R/get_function_names.R get_function_names
#> 5                     R/get_working_files.R  get_working_files
#> 6                                README.Rmd               <NA>
#> 7                          tests/testthat.R               <NA>
#> 8  tests/testthat/test-get_function_names.R               <NA>
#> 9   tests/testthat/test-get_working_files.R               <NA>
#> 10                     vignettes/outils.Rmd               <NA>
```
