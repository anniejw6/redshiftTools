<!-- README.md is generated from README.Rmd. Please edit that file -->
redshiftTools
=============

This is an R Package meant to easen the uploading of bulk data into Amazon Redshift.

Installation
------------

To install this package, you'll need to execute these commands:

``` r
install.packages(c('devtools', 'httr'))
devtools::install_github("RcppCore/Rcpp")
devtools::install_github("rstats-db/DBI")
devtools::install_github("rstats-db/RPostgres")
devtools::install_github("hadley/xml2")
install.packages("aws.s3", repos = c(getOption("repos"), "http://cloudyr.github.io/drat"))

remove.packages("data.table")                         # First remove the current version
install.packages("data.table", type = "source",
                 repos = "http://Rdatatable.github.io/data.table") # Then install devel version
devtools::install_github("anniejw6/redshiftTools", ref = 'refac')
```

Create your table
Then use `rs_replace_table`. 
