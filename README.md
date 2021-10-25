# Week-1-Activity-R-Markdown
Show in New Window

R 4.1.0·/cloud/project/
Console
Terminal
Close Terminal tab
Jobs
Close Jobs tab
R 4.1.0	·	/cloud/project/	
			

			

R version 4.1.0 (2021-05-18) -- "Camp Pontanezen"
Copyright (C) 2021 The R Foundation for Statistical Computing
Platform: x86_64-pc-linux-gnu (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under certain conditions.
Type 'license()' or 'licence()' for distribution details.

R is a collaborative project with many contributors.
Type 'contributors()' for more information and
'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or
'help.start()' for an HTML browser interface to help.
Type 'q()' to quit R.

> 
> 
> install.packages(ggplot2)
Error in install.packages : object 'ggplot2' not found
> install.packages("dplyr")
Installing package into ‘/cloud/lib/x86_64-pc-linux-gnu-library/4.1’
(as ‘lib’ is unspecified)
trying URL 'http://package-proxy/focal/src/contrib/dplyr_1.0.7.tar.gz'
Content type 'application/x-tar' length 1278969 bytes (1.2 MB)
==================================================
downloaded 1.2 MB

* installing *binary* package ‘dplyr’ ...
* DONE (dplyr)

The downloaded source packages are in
	‘/tmp/RtmphkZZ8d/downloaded_packages’
> install.packages("ggplot2")
Installing package into ‘/cloud/lib/x86_64-pc-linux-gnu-library/4.1’
(as ‘lib’ is unspecified)
trying URL 'http://package-proxy/focal/src/contrib/ggplot2_3.3.5.tar.gz'
Content type 'application/x-tar' length 4134212 bytes (3.9 MB)
==================================================
downloaded 3.9 MB

* installing *binary* package ‘ggplot2’ ...
* DONE (ggplot2)

The downloaded source packages are in
	‘/tmp/RtmphkZZ8d/downloaded_packages’
> install.packages("dplyr")
Installing package into ‘/cloud/lib/x86_64-pc-linux-gnu-library/4.1’
(as ‘lib’ is unspecified)
trying URL 'http://package-proxy/focal/src/contrib/dplyr_1.0.7.tar.gz'
Content type 'application/x-tar' length 1278969 bytes (1.2 MB)
==================================================
downloaded 1.2 MB

* installing *binary* package ‘dplyr’ ...
* DONE (dplyr)

The downloaded source packages are in
	‘/tmp/RtmphkZZ8d/downloaded_packages’
> 
> #The include = FALSE function hides both the code and output in my output document
> 
> #You need to install these packages first to be able to use the functions within them. You can install them from the Tools tab or write a new code chunk: install.packages("package_name"). 
> library(ggplot2)
> library(dplyr)

Attaching package: ‘dplyr’

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union

> #This next code chunk will make a plot in our output doc
> #Note, Each gray box below is a code chunk. You need to insert a code chunk and put your R code in it. By setting echo = FALSE. this comment and any code will not show in my output document. If it were TRUE, the comment and code would appear. 
> #The include = FALSE function hides both the code and output in my output document
> 
> #You need to install these packages first to be able to use the functions within them. You can install them from the Tools tab or write a new code chunk: install.packages("package_name"). 
> library(ggplot2)
> library(dplyr)
> #this next line is creating a subset called 'smaller' of the diamonds data
> smaller <- diamonds %>% 
+   filter(carat <= 2.5)
> #This next chunk is inline code. Inline code puts the text with the output of the function in my document.
> #This next code chunk will make a plot in our output doc
> smaller %>% 
+   ggplot(aes(carat)) + 
+   geom_freqpoly(binwidth = 0.01)
> #Once all of my code has been written, I click on the Knit button in the tool bar above to produce my document.
> #Note, Each gray box below is a code chunk. You need to insert a code chunk and put your R code in it. By setting echo = FALSE. this comment and any code will not show in my output document. If it were TRUE, the comment and code would appear. 
> #The include = FALSE function hides both the code and output in my output document
> 
> #You need to install these packages first to be able to use the functions within them. You can install them from the Tools tab or write a new code chunk: install.packages("package_name"). 
> library(ggplot2)
> library(dplyr)
> #this next line is creating a subset called 'smaller' of the diamonds data
> smaller <- diamonds %>% 
+   filter(carat <= 2.5)
> #This next chunk is inline code. Inline code puts the text with the output of the function in my document.
> #This next code chunk will make a plot in our output doc
> smaller %>% 
+   ggplot(aes(carat)) + 
+   geom_freqpoly(binwidth = 0.01)
> unlink("Anna Sample Markdown_cache", recursive = TRUE)
