
<!-- README.md is generated from README.Rmd. Please edit that file -->
# treefrog

<!-- badges: start -->
<!-- badges: end -->
## Installation

You can install the development version of treefrog like so:

``` r
# install.packages("devtools")
devtools::install_github("AnushaPB/treefrog")
```

## Example

``` r
library(treefrog)
library(here)
#> here() starts at /mnt/c/Users/Anusha/Documents/GitHub/treefrog

# examples
res <- generateDirectoryTree(here(), "filetree.txt", include_pattern = c("*.py", "*.R"), exclude_pattern = "html")
#> ├───DESCRIPTION                         #DESCRIPTION HERE
#> ├───[man]                               #DESCRIPTION HERE
#> │       ├───generateDirectoryTree.Rd    #DESCRIPTION HERE
#> ├───[R]                                 #DESCRIPTION HERE
#> │       ├───generateDirectoryTree.R     #DESCRIPTION HERE
#> └───README.Rmd                          #DESCRIPTION HERE
```

``` r
res <- generateDirectoryTree(here(), include_pattern = c("*.R"), fill_in = TRUE)
```
