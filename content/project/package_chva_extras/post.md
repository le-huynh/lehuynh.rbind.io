+++
showonlyimage = false
draft = false
image = "https://github.com/le-huynh/chva.extras/blob/master/man/figures/logo.png?raw=true"
title = "chva.extras"
weight = 4
description = "R/chva.extras: Supplementary Tools for Research"
+++

`R/chva.extras`*: Supplementary Tools for Climate and Health Research in VA*

<a href="https://le-huynh.github.io/chva.extras/" target="_blank">
<img align="right" alt="logo" width="150" src="https://github.com/le-huynh/chva.extras/blob/master/man/figures/logo.png?raw=true" />
</a>  

<a href="https://github.com/le-huynh/chva.extras/actions/workflows/R-CMD-check.yaml" target="_blank">
<img align="left" alt="r-cmd-check" style="margin-right: 5px;" src="https://github.com/le-huynh/chva.extras/actions/workflows/R-CMD-check.yaml/badge.svg" />
</a>  

<a href="https://lifecycle.r-lib.org/articles/stages.html#stable" target="_blank">
<img align="left" alt="lifecycle" style="margin-right: 5px;" src="https://img.shields.io/badge/lifecycle-stable-brightgreen.svg" />
</a>  

<a href="https://doi.org/10.5281/zenodo.14910966" target="_blank">
<img align="left" alt="doi" src="https://zenodo.org/badge/917932837.svg" />
</a>  

<br>

→ <a href="https://github.com/le-huynh/chva.extras" target="_blank">GitHub repository</a>  
→ <a href="https://le-huynh.github.io/chva.extras/" target="_blank">Package Website</a>  


`chva.extras` is a collection of supplementary functions and templates designed 
to support climate and health research in VA, including tools for data manipulation, 
analysis, and visualization, tailored to handle large datasets.  

<hr>

#### Installation

To get the latest in-development features, install the development
version from GitHub:

```
if(!requireNamespace("devtools", quietly = TRUE)) {
 install.packages("devtools")
}
devtools::install_github("le-huynh/chva.extras")
```

Additionally, this package is accessible for download via Zenodo with the DOI <a href="https://doi.org/10.5281/zenodo.14910966" target="_blank">10.5281/zenodo.14910967</a>.

#### Functions
See [Package index](https://le-huynh.github.io/chva.extras/reference/index.html) for full list of functions.  

1. Convert files to Parquet format  
- `get_parquet_arrow()`: Convert multiple files to Parquet format.  
- `get_parquet_by_chunk()`: Convert file to Parquet format by chunks.  

2. Support handy workflow
- `check_overview()`: Provide an overview of datasets.  
- `check_unique_value()`: Count unique values of a specified column.  
- `get_dataset()`: Get full working datasets as a named list of [Dataset](https://arrow.apache.org/docs/r/reference/Dataset.html) R6 objects.  
- `recode_values()`: Recode values based on grouping logic.  

For a comprehensive overview of the package's functions, check out the package website at  
<a href="https://le-huynh.github.io/chva.extras/" target="_blank">le-huynh.github.io/chva.extras/</a>.

<br/>

