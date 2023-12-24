+++
showonlyimage = false
draft = false
image = "img/project/proj_lehuynh_cover.png"
title = "lehuynh"
weight = 4
description = "R/lehuynh: Personal R package"
+++

`R/lehuynh`*: Personal R package*  

[<img align="left" alt="r-cmd-check" src="https://github.com/le-huynh/lehuynh/actions/workflows/R-CMD-check.yaml/badge.svg" />](https://github.com/le-huynh/lehuynh/actions/workflows/R-CMD-check.yaml)  

[<img align="left" alt="doi" src="https://zenodo.org/badge/389311777.svg" />](https://zenodo.org/doi/10.5281/zenodo.10421410)  

<br>

→ [GitHub repository](https://github.com/le-huynh/lehuynh)  


As a data enthusiast myself, I have always sought tools that streamline the data analysis process without compromising on flexibility or efficiency. 
Fueled by this quest, I embarked on the journey of crafting `lehuynh`. 
This package encapsulates a culmination of my passion for data and software development.  

`lehuynh` is an R package comprising a collection of miscellaneous R functions and templates that I find particularly useful. 
This package includes: 
- **Functions** pertaining to graphics, data importation, data transformation, and general utilities.  
- **Templates** designed for Exploratory Analysis, Bayesian modeling, and crafting scientific manuscripts.  

<hr>

#### Installation

`lehuynh` R package can be installed from GitHub using the following code:

```
if(!requireNamespace("devtools", quietly = TRUE)) {
 install.packages("devtools")
}
devtools::install_github("le-huynh/lehuynh")
```

Additionally, this package is accessible for download via Zenodo with the DOI [10.5281/zenodo.10421410](https://zenodo.org/doi/10.5281/zenodo.10421410).


#### Functions
- `ggsave_elsevier( )`: Save a plot using `ggplot2::ggsave( )`. Plot size follows instructions of Elsevier journals
- `import_data( )`: Import multiple .csv or .rds objects. The output is a *named* list of imported objects or separate objects in the .GlobalEnv.
- `import_excel( )`: Import excel file with multiple sheets. The output is a *named* list of imported sheets or separate dataframes in the .GlobalEnv. 
- `lehuynh_theme( )`: Personal ggplot2 theme (white background, black axis, black text, etc.)
- `MinMaxScaling( )`: Min-max normalization (min = 0, max = 1)
- `new_project( )`: Create a [project](https://github.com/SchlossLab/new_project) for reproducible purpose
- `ppc_brms( )`
- `tidytuesday( )`: Create a new folder for [#tidytuesday](https://github.com/rfordatascience/tidytuesday) challenge
- `tsi( )`: Calculate TSI (Trophic state index) [(Carlson, 1977)](https://doi.org/10.4319/lo.1977.22.2.0361)


#### Templates
- `draft_elsevier`: Creating an Rmarkdown manuscript for Elsevier journals [(example)](https://github.com/le-huynh/writing_journal_article_in_rmarkdown)
- `lehuynh_Bayes_brms`: Basic steps to fit, check, and interpret a Bayesian model via `brms` package
- `lehuynh_EA`: Basic steps to do Exploratory Analysis


