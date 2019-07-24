#######
Jupyter
#######

`Project Jupyter <https://jupyter.org/index.html>`_ is an open-source project intended to support
interactive scientific computing across numerous languages. 

*Documentation*: `<https://jupyter.readthedocs.io/en/latest/>`_

.. tip::
	Scared of commitment? To try Jupyter without installation, click `here <https://jupyter.org/try>`__.

.. toctree::	
	:caption: Table of Contents
	:maxdepth: 3
	
	jupyter

****************
Jupyter Notebook
****************

The `Jupyter Notebook <https://jupyter-notebook.readthedocs.io/en/stable/#>`_ is an open-source web application which
provides an interactive environment that smoothly integrates live code, images, equations, data visualization, interactive
widgets, and text. 

.. note::
	Jupyter is not exclusive to Python - it supports over 40 languages, including R, Java, and MATLAB. IPython is the default kernel
	of Jupyter Notebook but other kernels can be installed to enable the use of other languages within Jupyter.
	
	Check out the list of available kernels `here <https://github.com/jupyter/jupyter/wiki/Jupyter-kernels>`__.

.. todo::
	ipywidgets, a note about latex
	
Tools
========

nbviewer
--------

`nbviewer <https://nbviewer.jupyter.org/>`_ renders Jupyter Notebooks in a browser. 

nbconvert
---------

`nbconvert <https://nbconvert.readthedocs.io/en/latest/index.html#>`_ converts Jupyter Notebooks (.ipynb files) to
other formats, including HTML and PDF.

.. hint::
	Installing Jupyter (``pip install jupyter``) also installs nbconvert. To use nbconvert from the 
	command line, enter the following command in the directory in which the notebook is stored.
	
	.. highlight:: console
	
	::
	
		$ jupyter nbconvert --to format notebook.ipynb
		
	Simply replace ``format`` wtih the desired format and ``notebook.ipynb`` with the notebook file.
	
.. tip::
	Saving as different formats is also possible within Jupyter. To see the available formats:
	
		* In Jupyter Notebook, 
		
		  	click on :guilabel:`File` then hover over :guilabel:`Download as`.
			
		* In Jupyter Lab, 
		
			click on :guilabel:`File` then hover over :guilabel:`Export Notebook As...`.
			
***********
Jupyter Lab
***********

******
Syzygy
******

`Syzygy <https://intro.syzygy.ca/>`_ is a service provided by the Pacific Insittute for the Mathematical Sciences (PIMS),
Compute Canada, and Cybera that launches Jupyter notebooks in a browser. It is accessed 
by logging in with a CWL through `<https://ubc.syzygy.ca/>`_. 

.. note::

	Each user is allocated 1GB of space.

 