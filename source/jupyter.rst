#######
Jupyter
#######

`Project Jupyter <https://jupyter.org/index.html>`_ is an open-source project intended to support
interactive scientific computing across numerous languages. 

*Documentation*: `<https://jupyter.readthedocs.io/en/latest/>`_

.. tip::
	Scared of commitment? To try Jupyter without installation, click `here <https://jupyter.org/try>`__.

.. contents:: Table of Contents
	:depth: 3

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

LaTeX
=====

Jupyter Notebooks can include inline and displayed mathematical equations written in LateX.

`LaTeX <https://www.latex-project.org/>`_ is used to typeset mathematical notation in scientific documents.

- The Jupyter Notebook documentation has a brief section on `LaTeX equations <https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html#LaTeX-equations>`_.

- For the basics of LaTeX, `An Introduction to Using TeX in the Harvard Mathematics Department <http://www.math.harvard.edu/texman/>`_
  is a concise and useful reference written by R. Kuhn, R. Scott, and L. Andreev.

- A list of `LaTeX Math Symbols <http://web.ift.uib.no/Teori/KURS/WRK/TeX/symALL.html>`_ prepared by L. Kocbach.

.. admonition:: Example of use
	
	In a Markdown cell,
		
		.. code-block:: python

			The Nernst Equation is as follows
			$$E_x = \frac{RT}{zF}ln{\frac{[X]_o}{[X]_i}}$$

			where $R$ is the gas constant, $T$ the temperature, $z$ the valence of the ion, $F$ the Faraday 
			constant, and $[X]_o$ and $[X]_i$ the concentrations of the ion outside and inside the cell. 
		
	where ``$$`` and ``$`` indicate the start and end of a displayed and inline equation respectively. 
	
	This produces
		
	.. image:: /Images/nernst.png
		:width: 686px
		:height: 243px
		:scale: 70 %
		:alt: Nernst equation
		:align: center
		
ipywidgets
==========

`ipywidgets <https://ipywidgets.readthedocs.io/en/stable/user_install.html#with-pip>`_ are interactive HTML
widgets that can be used to build GUIs within Jupyter Notebooks. Available widgets include buttons, sliders,
textboxes, and checkboxes.

.. hint::

	.. code-block:: console
	
		$ pip install ipywidgets
		$ jupyter nbextension enable --py widgetsnbextension
		
	To use:
	
	.. highlight:: python
	
	::
		
		import ipywidgets as widgets
			
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
		
	Replace ``format`` wtih the desired format and ``notebook.ipynb`` with the notebook file.
	
.. tip::
	Saving as different formats is also possible within Jupyter. To see the available formats:
	
		* In Jupyter Notebook, 
		
		  	click on :guilabel:`File` then hover over :guilabel:`Download as`.
			
		* In Jupyter Lab, 
		
			click on :guilabel:`File` then hover over :guilabel:`Export Notebook As...`.
			
***********
Jupyter Lab
***********

`Jupyter Lab <https://jupyterlab.readthedocs.io/en/stable/index.html>`_ is the web-based user interface intended
to replace Jupyter Notebook. It has all the classic features of its predecessor plus some cool new ones, most notably it offers
a flexible and unified workspace that can include a code console, terminal, text editor, and Notebook.

******
Syzygy
******

`Syzygy <https://intro.syzygy.ca/>`_ is a service provided by the Pacific Insittute for the Mathematical Sciences (PIMS),
Compute Canada, and Cybera that launches Jupyter notebooks in a browser. It is accessed 
by logging in with a CWL through `<https://ubc.syzygy.ca/>`_. 

.. note::

	Each user is allocated 1GB of space.

 