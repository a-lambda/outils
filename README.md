
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
#>  [1] "dev/0-dev_history.Rmd"                   
#>  [2] "dev/flat_my_sql.Rmd"                     
#>  [3] "dev/flat_outils.Rmd"                     
#>  [4] "R/get_function_names.R"                  
#>  [5] "R/get_working_files.R"                   
#>  [6] "R/my_con.R"                              
#>  [7] "README.Rmd"                              
#>  [8] "tests/testthat.R"                        
#>  [9] "tests/testthat/test-get_function_names.R"
#> [10] "tests/testthat/test-get_working_files.R" 
#> [11] "tests/testthat/test-my_con.R"            
#> [12] "vignettes/my_sql.Rmd"                    
#> [13] "vignettes/outils.Rmd"

get_function_names(get_working_files())
#>              fonction                                  fichier
#> 1                <NA>                    dev/0-dev_history.Rmd
#> 2              my_con                      dev/flat_my_sql.Rmd
#> 3   get_working_files                      dev/flat_outils.Rmd
#> 4  get_function_names                      dev/flat_outils.Rmd
#> 5  get_function_names                   R/get_function_names.R
#> 6   get_working_files                    R/get_working_files.R
#> 7              my_con                               R/my_con.R
#> 8                <NA>                               README.Rmd
#> 9                <NA>                         tests/testthat.R
#> 10               <NA> tests/testthat/test-get_function_names.R
#> 11               <NA>  tests/testthat/test-get_working_files.R
#> 12               <NA>             tests/testthat/test-my_con.R
#> 13               <NA>                     vignettes/my_sql.Rmd
#> 14               <NA>                     vignettes/outils.Rmd

con <- my_con()
class(con)
#> [1] "PqConnection"
#> attr(,"package")
#> [1] "RPostgres"
```
