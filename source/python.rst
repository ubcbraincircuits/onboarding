######
Python
######

Python is a high-level, interpreted programming language that is widely used for 
scientific analysis and computation.  

.. toctree::	
	:caption: Table of Contents
	:maxdepth: 3
	
	python

************
Installation
************

Mac OS X and some Linux distributions have Python installed by default.
	
Windows users can download the latest version of Python from the `website <https://www.python.org/downloads/>`_.

Once installation is done, click the Python application file again (it should be in the 
Downloads folder as python-<version_number>.exe). A window will pop up. Click on :guilabel:`Modify`
then select :guilabel:`Next`, which leads to :guilabel:`Advanced Options`. Tick the box labeled :guilabel:`Add Python
to environment variables` then click :guilabel:`Install`. Python will now be avaliable in both Command
Prompt and Windows PowerShell. 

To verify installation or to check the version of Python on your system, open a Terminal window (Mac OS X) 
or Command Prompt (Windows) and enter the command below.

.. code-block:: console

		$ python --version
		
*************
Documentation
*************

Python Standard Library
=======================

The `Python Standard Library <https://docs.python.org/3/library/index.html#library-index>`_ contains descriptions 
of built-in functions, constants, types, exceptions, and modules.

PEP 8 
=====

`PEP 8 <https://www.python.org/dev/peps/pep-0008/>`_ is the official Python style guide. It outlines Python coding 
conventions to promote readability of code and consistency within and between projects. 

.. tip::

	Adopt good coding habits early. To check that your code is compliant with PEP 8 conventions, run 
	:ref:`pycodestyle<pycodestyle>` on your script.
	
Python Package Index (PyPI)
===========================

The `Python Package Index (PyPI) <https://pypi.org/>`_ is a repository of Python packages. 

.. Important::
	``pip`` is the Python package installer program. To install a package,
	enter the command ``pip install <package_name>`` into Terminal or Command Prompt. 
	
The packages listed here form the basis of most data analysis and processing. 

IPython
-------

`IPython <https://ipython.org/>`_ is an interactive Python shell. It is best
for exploratory and demonstrative purposes, like quickly testing functions or playing around with 
new commands.

*Documentation*: `<https://ipython.readthedocs.io/en/stable/>`_

.. admonition:: Example of use

	In a Terminal or Command Prompt window,

	.. image:: /Images/ipython.png
	   :width: 709px
	   :height: 158px
	   :scale: 100 %
	   :alt: x = 5+2 in IPython
	   :align: center

.. tip::
	Try using IPython to go through the examples in this page.
	
NumPy 
-----

`NumPy <https://www.numpy.org/>`_ is a library for scientific computation, which includes
support for array and matrix operations, as well as mathematical functions. 

*Documentation*: `NumPy Manual <https://docs.scipy.org/doc/numpy/index.html>`_

.. Important::
	To enable the use of NumPy and other packages during a session, it must be *imported*. 
	For ease of use, it is standard for most modules to be imported using an abbreviation. 
	For NumPy, it is typically "np".
	
	.. highlight:: python
	
	::
	
		>>> import numpy as np
		 	 
.. admonition:: Example of use

	Calculate the average potential of a membrane at rest. Suppose the data was stored in
	a variable called potential, which is an array of voltages in units of millivolts. 
	
	.. highlight:: python
	
	::
	
		>>> type(potential) # check that potential is indeed an array
		numpy.ndarray
		>>> mean = np.mean(potential)
		>>> mean
		-70.232
		
.. Note::
	Comments in Python begin with ``#``.
	
Matplotlib
----------

`Matplotlib <https://matplotlib.org/>`_ is a 2D plotting library. The pyplot API `matplotlib.pyplot <https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.html#module-matplotlib.pyplot>`_
is a collection of MATLAB-like functions intended for simple plots. 

*Documentation*: `User's Guide <https://matplotlib.org/users/index.html>`_

.. hint:: 

	.. highlight:: python
	
	::
	
		>>> import matplotlib.pyplot as plt
		
SciPy
-----

pandas
------

pycodestyle
-----------

pycodestyle is the Python style guide checker. It was formerly known as pep8.

*Documentation*: `<https://pycodestyle.readthedocs.io/en/latest/>`_

.. admonition:: Example of use

	Note the use of the ``more`` command to see the contents of example.py. 

	.. highlight:: console
	
	::
		
		$ more example.py
		a="Welcome to the Brain Circuits Cluster!"
		
		print(a)
		
		$ python example.py
		Welcome to the Brain Circuits Cluster!
		
		$ pycodestyle example.py
		example.py:1:2: E225 missing whitespace around operator
		
	A space must be added before and after the equal sign. Modify the script and run it through
	pycodestyle again.
	
	.. highlight:: console
	
	::
	
		$ more example.py
		a = "Welcome to the Brain Circuits Cluster!"
		
		print(a)
		
		$ pycodestyle example.py
		
		$ 
		
	All is well!
		
.. todo::
	ipython, numpy, matplotlib, scipy 

*********
Tutorials
*********

******************
Anaconda Navigator
******************

Anaconda Navigator is a desktop graphical user interface (GUI) that can launch commonly used Python applications, such as Spyder, JupyterLab, 
and Jupyter notebook. 

Installation instructions are available here:
	- `Windows <https://docs.anaconda.com/anaconda/install/windows/>`_
	- `macOS <https://docs.anaconda.com/anaconda/install/mac-os/>`_
	- `Linux <https://docs.anaconda.com/anaconda/install/linux/>`_