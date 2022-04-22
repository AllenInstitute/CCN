# CCN

### Overview

This repository contains an R library to generate the standardized **Common Cell type Nomenclature (CCN)** for a cell type taxonomy, and is a companion repository of **[AllenInstitute/nomenclature](https://github.com/AllenInstitute/nomenclature)**.  More general information about what the CCN is and why it's important can be found [on our website, here](https://portal.brain-map.org/explore/classes/nomenclature), with and updated version **now published [on eLife](https://elifesciences.org/articles/59928)**.

Specific details of how to apply the CCN to your cell type taxonomy can be found at **[AllenInstitute/nomenclature](https://github.com/AllenInstitute/nomenclature)** or by typing `browseVignettes("CCN")` in R after installing this library.

### Installation

Install prerequisites (if not already installed):
```
packages <- c("remotes","jsonlite","data.table","ggplot2","dendextend","dplyr","BiocManager")
packages <- packages[!(packages %in% installed.packages()[,"Package"])]
if(length(packages)>0) install.packages(new.packages, repos='http://cran.us.r-project.org')
BiocManager::install("rols", update=FALSE)
```

Install `CCN` and its vignettes:
```
remotes::install_github("AllenInstitute/CCN", build_vignettes = TRUE)
```

### License

The license for this package is available on Github at: https://github.com/AllenInstitute/CCN/blob/master/LICENSE

### Level of Support

We are planning on occasional updating this tool with no fixed schedule. Community involvement is encouraged through both issues and pull requests.

### Contribution Agreement

If you contribute code to this repository through pull requests or other mechanisms, you are subject to the Allen Institute Contribution Agreement, which is available in full at: https://github.com/AllenInstitute/CCN/blob/master/CONTRIBUTION
