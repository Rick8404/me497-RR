
download resource and data files
================================

Our test lab has provided us two files: an image of the test setup, and a data set. Both files are available online. To retrieve these files and place them in the appropriate directories:

-   Make sure you have a live Internet connection
-   Launch your RStudio project.
-   To download the *image*, copy these lines of R code, paste into the Console (lower left pane of the RStudio interface), and `Enter`.

``` r
url <- "https://github.com/DSR-RHIT/me497-RR/tree/master/resources"
destination <- "resources/load-cell-setup-786x989px.png"
download.file(url, destination, mode = "wb")
```

-   To download the *data*, copy these lines of R code, paste into the Console, and `Enter`.

``` r
url <- "https://github.com/DSR-RHIT/me497-RR/tree/master/data"
destination <- "data/007_wide-data.csv"
download.file(url, destination)
```

Learn R

-   `<-` is the R assignment operator
-   `download.file()` downloads a file from the Internet to your machine
-   `destination` is a relative path with respect to your working directory and includes the filename under which we save the file to our local machine.
-   `mode = wb` mode is for *binary* files (images and other non-text files)

learning the software
---------------------

As shown above in the "Learn R" list, whenever I show you some new code or markup, I give a brief description of what the code is doing. To get the most out of the tutorials, please take the time to study those remarks carefully.

check yourself
--------------

Your directories should contain these files:

    data\
      `-- 007_wide-data.csv

    reports\

    resources\
      `-- load-cell-setup-786x989px.png 
      
    results\
      
    scripts\

If your download was not successful, navigate to <https://github.com/DSR-RHIT/creating-reproducible-reports/tree/gh-pages/resources/downloads> and follow the instructions.

push to github
--------------

For reproducibility, the data file and the image file are pushed to GitHub.

These steps can only be taken if you have successfully set up RStudio, Git, and GitHub to talk to each other.

-   In RStudio, in the upper-right pane, select the `Git` tab
-   Check the `Staged` box for the `data/` directory, the `resources/` directory, the `007_wide-data.csv`data file and the `load-cell-setup-786x989px.png` image file.

-   Click the `Commit` button
-   Type a commit message, e.g., `data and image upload`
-   `Commit`
-   `Close`
-   `Push`
-   `Close`

check yourself
--------------

Online, navigate to your project repo on GitHub. There you should find a data folder containing the CSV file and a resources folder containing the PNG file.

------------------------------------------------------------------------

[main page](../README.md)
