retina-subunits
===============

Code for fitting subunit models

How to use
----------

First create a location and set appropriate paths in `data/loadData.m`

Data sets must be mat files called 

Load a dataset

	dat = loadData('location','2011-10-25-5/data001-0')

Perform an STC (and LN) analysis of cells of a particular type from a data set

	batchAnal('laptop','2011-10-25-5/data001-0','off midget','stc',1,0,0.33)

Perform subunit fits

	batchAnal('laptop','2011-10-25-5/data001-0','off midget','subunit',1,0,0.33)

Generate and save plots of subunit fits

	batchAnal('laptop','2011-10-25-5/data001-0','off midget','subunit',0,1,0.33)
