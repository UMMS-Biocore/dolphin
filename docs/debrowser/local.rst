*******************
Local Install Guide
*******************

Quick Local Install
===================

Running these simple command will launch the DEBrowser within your local
machine.

Before you start;
First, you will have to install R and/or RStudio.
(On Fedora/Red Hat/CentOS, these packages have to be installed;
openssl-devel, libxml2-devel, libcurl-devel, libpng-devel)

**Installation instructions from source:**

1. Install the dependencias by running source command on attached bioC_install.R script in R or RStudio. 

        source("./bioC_install.R")

2. Install debrowser using the command below

        R CMD INSTALL debrowser_0.99.0.tar.gz

3. Start R and load the library

        library(debrowser)

4. Start DE browser

        startDEBrowser()