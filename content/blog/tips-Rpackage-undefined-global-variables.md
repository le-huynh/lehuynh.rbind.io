+++
showonlyimage = false
draft = false
image = "img/tips.png"
title = "Undefined global variables"
weight = 3
description = "NOTE when creating new function in Rpackage"
+++

#### NOTE
I am creating a new function in my Rpackage. 
After running `devtools::check()`, I get this NOTE:  

```
checking R code for possible problems ... NOTE
  function_name1: no visible binding for global variable 'value1'
  function_name2: no visible binding for global variable 'value2'
  Undefined global variables:
    value1 value2
```

#### Solution
Create a file `globals.R` in the `R` folder, listing undefined global variables:  

```
utils::globalVariables(c("value1", "value2"))

```


