<!-- badges: start -->
[![CRAN Status](https://www.r-pkg.org/badges/version/myClim)](https://cran.r-project.org/package=myClim)
[![](http://cranlogs.r-pkg.org/badges/grand-total/myClim)](https://cran.r-project.org/package=myClim)
[![CRAN RStudio mirror downloads](http://cranlogs.r-pkg.org/badges/myClim)](https://cran.r-project.org/package=myClim)
<!-- badges: end -->

# Install

Install from CRAN:

```R
install.packages("myClim")
```

Or install the latest development version with dependencies:
```R
requiered_packages <- c("stringr", "lubridate", "tibble", "dplyr", "purrr",
                        "ggplot2", "ggforce", "viridis", "runner", "rmarkdown",
                        "knitr", "kableExtra", "tidyr", "plotly", "zoo", "vroom")
missing_packages <- requiered_packages[!(requiered_packages %in% installed.packages()[,"Package"])]
if(length(missing_packages)) install.packages(missing_packages)

# optional package rTubeDB
remotes::install_github('environmentalinformatics-marburg/tubedb/rTubeDB')

# installation of myClim package
install.packages("http://labgis.ibot.cas.cz/myclim/myClim_latest.tar.gz", repos=NULL, build_vignettes=TRUE)
```
# Documentation & user manual
* [manual - functions documentation](http://labgis.ibot.cas.cz/myclim/reference/index.html)   
* [tutorial - vignette](http://labgis.ibot.cas.cz/myclim/articles/myclim-demo.html)

# Source code of package
* [GitHub repository](https://github.com/ibot-geoecology/myClim)   
