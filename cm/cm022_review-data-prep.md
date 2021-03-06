
review of tools for preparing data
==================================

Here, we briefly review the suite of tools we used in the Project 1 tutorials for preparing data for analysis.

The packages we used are

``` r
library(dplyr)
library(tidyr)
library(stringr)
library(readr)
library(tibble)
```

These packages are all written by Hadley Wickham, who also happens to be the author of the ggplot2 package and a senior data scientist at RStudio. And quite a nice fellow in person as well.

If you subscribe to the [RStudio webinar notifications](https://www.rstudio.com/resources/webinars/), you can receive online notices of free webinars put on by Hadley and other folks at RStudio. I recommend it.

input/output
------------

-   `read_csv()`
-   `write_csv()`

examining the data structure
----------------------------

-   `str()` displays the internal structure of an R object
-   `glimpse()` like `str()` applied to a data frame but it tries to show you as much data as possible
-   `head()` returns the first part of an R object
-   `tail()` returns the last part of an R object
-   `summary()` returns a statistical summary of an object
-   `colnames()` returns column names
-   `nrow()` returns the number of rows of a data frame
-   `typeof()` tells us what the object is
-   `attributes()` yields metadata about the object
-   `class()`

basic functions in R
--------------------

-   `max()` and `min()` are R functions that do the obvious
-   `ab()` absolute value
-   `log10()` for base 10, `log()` for base *e*
-   `<=` (less than or equal) and `>=` (greater than or equal) are logical operators that return logical values TRUE or FALSE

subsetting data
---------------

-   `select()` keeps only the variables (columns) you list
-   `filter()` keeps the rows listed
-   `[]` brackets, as in `variable_name[indices]`
-   `[[]]` double brackets subsets a list and returns its components
-   `which()` yields the TRUE indices of a logical object
-   `$` extract

editing strings
---------------

-   `tolower()` strings to lower case
-   `str_replace()`
-   `str_detect()`
-   `str_c()` concatenate strings
-   `separate()` turns one column of strings into multiple columns of strings

reshaping data
--------------

-   `c()` concatenate elements to create a vector
-   `gather()` collapses multiple columns into two columns: one column of the former column headings (the "keys") and one column of the former column entries (the "values"). All other columns are duplicated (copy/paste downward in chunks) as needed.
-   `mutate()` creates a new column in a data frame (can also be used to overwrite an existing column)
-   `unname()` removes the names from named numbers
-   `frame_data()` create a data frame row by row
-   `data.frame()` convert object to data frame
-   `arrange()` arrange by row entries
-   `select()` arrange by column names

display results
---------------

-   `kable()`
-   `print()` write an object in the Console

control of code execution
-------------------------

-   `stopifnot()` stops the code execution and produces an error message if any argument returns FALSE

------------------------------------------------------------------------

[main page](../README.md)
