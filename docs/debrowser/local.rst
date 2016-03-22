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

Make sure to download the DEBrowser tar `here<https://github.com/UMMS-Biocore/debrowser/archive/debrowser0.99.0.tar.gz>`_ or you can
download from our `github repository.<https://github.com/UMMS-Biocore/debrowser>`_

**Installation instructions from source:**

1. Install the required dependencias by running the following commands in R or RStudio. 

        ### Packages for R.

		install.packages("ggvis")

		install.packages("ggplot2")

		install.packages("RColorBrewer")

		install.packages("DT")

		install.packages("gplots")

		install.packages("devtools")


	### BioC Packages for R.
		
		source("http://www.bioconductor.org/biocLite.R")

		biocLite()

		biocLite("clusterProfiler")

		biocLite("ReactomePA")

		biocLite("shiny")

		biocLite("DESeq2")

		biocLite("annotate")

		biocLite("AnnotationDbi")

		biocLite("org.Hs.eg.db")

		biocLite("DOSE")

		biocLite("edgeR")


2. Install debrowser using the command below

        R CMD INSTALL debrowser_0.99.0.tar.gz

3. Start R and load the library

        library(debrowser)

4. Start DE browser

        startDEBrowser()
