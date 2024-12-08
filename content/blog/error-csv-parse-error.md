+++
showonlyimage = false
draft = false
image = "img/error.png"
title = "CSV parse error: Row #20241208: Expected 111 columns, got 110"
weight = 3
description = " "
+++


#### Error
I encountered the following error when using `arrow::read_csv_arrow()` or `arrow::open_dataset()`.  

```
Error: Invalid: CSV parse error: Row #20241208: Expected 111 columns, got 110: 
"col1","col1","col3","col4","col5"," ...
```


#### Solution
##### Reason
At row 20241208, there might be unexpected characters in one or more columns 
that interfere with detecting the delimiter of the CSV file. 
These could include `""`, `\"`, a blank space, or a combination of punctuation marks.  

I have not found a perfect solution for this error. 
The approach may vary depending on the goal after importing the data into R. 
In my case, the CSV file was very large, and I wanted to convert it into 
multiple Parquet files for storage and efficient querying later. 
However, the file could not be converted unless it was read correctly.  
Here are the steps I followed:

##### Step 1 (Optional)
Extract row 20241208 to identify the problematic characters.  
Big thanks to <a href="https://huynhvu.com/" target="_blank">Dr. Huynh Vu</a> 
for helping with the <a href="https://github.com/vuh95" target="_blank">Python code</a>. 
If you're into Python and data stuff, you should totally check out <a href="https://huynhvu.com/" target="_blank">his blog</a>
—he’s got tons of great tips and tricks!

##### Step 2
Use `data.table::fread()` to read the CSV file into R, and replace the problematic characters if necessary. 
This function does not fail due to parsing errors. 
The downside is that your computer's RAM must be large enough to handle `fread()` for in-memory data import.

##### Step 3
Convert the cleaned data into Parquet format.

#### References
<a href="https://umatter.github.io/BigData/" target="_blank">Big Data Analytics</a> by Ulrich Matter.







