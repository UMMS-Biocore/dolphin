***************************
DEBrowser Quick-start Guide
***************************

This guide is a quick walkthrough for the DESeq Browser from start to finish.

Getting Started
===============

First off, we need to head to the DEBrowser webpage at this url:

http://labkey.umassmed.edu/debrowser/

Once you've made your way to the website, you will be greeted with this tab on the left:

.. image:: debrowser_pics/input_tab.png
	:align: center
	
To begin the DESeq process, you will need to select your Data file (CSV format) to be analyzed using DESeq.

This selection is under the 'Choose CSV File'.

Once you've selected your file and the upload has completed, you will then be able to select your conditions in which you wish to compare using DESeq.

.. image:: debrowser_pics/file_load.png
	:align: center
	
.. image:: debrowser_pics/condition_selection.png
	:align: center
	
Once you've selected your conditions, you can then hit 'Run DESeq!' to begin.

Analyzing The Results
=====================

Once DESeq has finished and the results have been uploaded into DEBrowser, the initial scatterplot of the results will be uploaded.

.. image:: debrowser_pics/scatter_plot.png
	:align: center
	
You can hover over the scatterplot points to display more information about the point selected.  A few bargraphs will be generated for the user to view as soon as a scatterplot point is hovered over.

.. image:: debrowser_pics/bargraph.png
	:align: center
	
.. image:: debrowser_pics/bar_plot.png
	:align: center
	
You can also select a specific region within the scatter plot and zoom in on the selected window.

.. image:: debrowser_pics/scatter_plot_selection.png
	:align: center
	
Once you've selected a specific region, a new scatterplot of the selected area will appear on the left

.. image:: debrowser_pics/scatter_plot_zoom.png
	:align: center
	
You also have a wide array of options when it comes to fold change cut-off levels, padj cut-off values, and up/down regulated genes.

.. image:: debrowser_pics/filters.png
	:align: center
	
You can also download the results in CSV or TSV format by selecting your 'File type' and clicking the 'download' button once you've ran DESeq.

Additional Plots/Tables
=======================

After DESeq has run, and you've had some time to play with the initial plots generated, You may notice the additional tabs above the plots.

.. image:: debrowser_pics/info_tabs.png
	:align: center
	
These tabs display additional plots or tables based on your current padj/fold-change cut-off values.

By selecting additional plots, you will be shown additional plots based on the 'Additional Plots' selection on the left tab.

The first selection, 'All2All', displays an all-to-all plot of your conditions slected.  As you change the padj and fold-change cutt-off values, the data in these plots will also change!

.. image:: debrowser_pics/all2all.png
	:align: center

Additionally, you can choose a specific dataset to display within these plots.  You can even use the datapoints you selected from the scatterplot on the plot page to be displayed in these additional plots/tables.

.. image:: debrowser_pics/dataset_choose.png
	:align: center
	
The second additional plot is the heatmap generated based on your dataset.

.. image:: debrowser_pics/heatmap.png
	:align: center

In addition to these exciting additional plots, you also have access to the data generated within table form.

The data generated is also sorted based on the following datasets:

* All Detected
* Up Regulated
* Down Regulated
* Selected scatterplot points

.. image:: debrowser_pics/datatable.png
	:align: center

More Tools
==========

We're creating more plots and graphs, but they're currently under construction!

In the meantime, enjoy the DESeq Browser!

	