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

#### Functions
- `check_overview( )`: Provide an overview of datasets with the number of rows, columns, and a flag indicating whether the column names across datasets are consistent.
- `check_unique_value()`: Count the unique values of a specified column.
- `check_unique_value_overview()`: Check the consistency of unique values within a specified column across multiple datasets.
- `get_dataset()`: Get full working datasets as a named list of [Dataset](https://arrow.apache.org/docs/r/reference/Dataset.html) R6 objects.
- `get_parquet_arrow()`: Convert multiple files to Parquet format.
- `get_parquet_by_chunk()`: Convert file to Parquet format by chunks.

For a comprehensive overview of the package's functions, check out the package website at  
<a href="https://le-huynh.github.io/chva.extras/" target="_blank">le-huynh.github.io/chva.extras/</a>.

<br/>

