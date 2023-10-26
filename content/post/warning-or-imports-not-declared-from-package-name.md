+++
showonlyimage = true
draft = false
image = "img/warning_red.png"
date = "2021-10-02"
title = "Warning: ''::'' or '':::'' imports not declared from: `package_name`"
weight = 2
description = "Warning: new function in Rpackage"
+++

#### Warning
I am creating a new function in my Rpackage. 
After running `devtools::check()`, I get this WARNING:  

```
checking dependencies in R code ... WARNING
'::' or ':::' imports not declared from:
  ‘dplyr’ 
```

#### (possible) Solution
Add `dplyr` to `Imports` in the `DESCRIPTION` file.  

```
usethis::use_package("dplyr")
#> Adding dplyr to Imports
#> Refer to functions with dplyr::fun()
```

#### Further information
[Dependencies: What does your package need?](https://r-pkgs.org/description.html#dependencies), 
_R Packages_ by  Hadley Wickham and Jenny Bryan  


