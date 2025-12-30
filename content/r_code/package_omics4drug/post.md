+++
showonlyimage = false
draft = false
image = "https://github.com/le-huynh/omics4drug/blob/main/man/figures/logo.png?raw=true"
title = "omics4drug"
weight = 3
description = "R/omics4drug: An R toolkit for Mass Spectrometry-based Proteomics and Phosphoproteomics data analysis"
+++

`R/omics4drug`*: An R toolkit for Mass Spectrometry-based Proteomics and Phosphoproteomics data analysis*

<a href="https://yen-kim.github.io/omics4drug/" target="_blank">
<img align="right" alt="logo" width="150" src="https://github.com/le-huynh/omics4drug/blob/main/man/figures/logo.png?raw=true" />
</a>  

<a href="https://github.com/yen-kim/omics4drug/actions/workflows/R-CMD-check.yaml" target="_blank">
<img align="left" alt="r-cmd-check" style="margin-right: 5px;" src="https://github.com/yen-kim/omics4drug/actions/workflows/R-CMD-check.yaml/badge.svg" />
</a>  

<a href="https://lifecycle.r-lib.org/articles/stages.html#stable" target="_blank">
<img align="left" alt="lifecycle" style="margin-right: 5px;" src="https://img.shields.io/badge/lifecycle-stable-brightgreen.svg" />
</a>  

<a href="https://doi.org/10.5281/zenodo.17117623" target="_blank">
<img align="left" alt="doi" src="https://zenodo.org/badge/1056782986.svg" />
</a>  

<br>

→ <a href="https://github.com/yen-kim/omics4drug" target="_blank">GitHub repository</a>  
→ <a href="https://yen-kim.github.io/omics4drug/" target="_blank">Package Website</a>  


`omics4drug` is designed for the analysis and visualization of 
Mass Spectrometry-based phosphoproteomics and proteomics data in drug discovery. 
The package provides functions for quality control, normalization, 
pathway enrichment analysis, and drug-target prediction.  

<hr>

#### Installation

To get the latest in-development features, install the development
version from GitHub:

```
if(!requireNamespace("devtools", quietly = TRUE)) {
 install.packages("devtools")
}
devtools::install_github("yen-kim/omics4drug")
```

This package is also accessible for download via Zenodo with the DOI <a href="https://doi.org/10.5281/zenodo.17117623" target="_blank">10.5281/zenodo.17117623</a>.

#### Functions
See <a href="https://yen-kim.github.io/omics4drug/reference/index.html" target="_blank">Package index</a> 
for full list of functions.  

1.  Data Processing and Quality Control
- `get_count_phosphosite()`: Counts and visualizes the number of unique
  phosphosites per sample or group, often based on a probability
  threshold.  
- `get_count_protein()`: Counts and visualizes the number of unique
  protein groups per sample or group.  
- `get_cv()`: Calculates and visualizes the coefficient of
  variation (CV) for a given dataset, useful for assessing data
  variability and quality.
- `get_sty()`: Calculates and visualizes the count and percentage of
  phosphorylation sites (Serine (S), Threonine (T), Tyrosine (Y)).

2.  Data Normalization
- `get_norm_phos()`: Normalizes phosphosite intensity data to account
  for variations between samples.
- `get_norm_prot()`: Normalizes protein group intensity data.

3.  Functional and Pathway Enrichment Analysis
- `get_GO()`: Performs Gene Ontology (GO) enrichment analysis to
  identify biological processes, molecular functions, or cellular
  components that are overrepresented in your data.
- `get_KEGG()`: Performs KEGG pathway enrichment analysis to determine
  which biological pathways are significantly impacted.

4.  Kinase and Drug Prediction
- `get_KSEA()`: Performs Kinase Substrate Enrichment Analysis (KSEA) to
  predict the activity of kinases based on the phosphorylation of their
  substrates.
- `get_inhibitor()`: Predicts which drugs might target the kinases
  identified in your analysis, using an external database.

5.  Others
- `get_annotation()`: Map Gene Identifiers

For a comprehensive overview of the package's functions, check out the package website at  
<a href="https://yen-kim.github.io/omics4drug/" target="_blank">yen-kim.github.io/omics4drug</a>.

<br/>

