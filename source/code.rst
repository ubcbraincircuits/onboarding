##########################
Beginner's Guide to Coding
##########################

.. toctree::	
	:caption: Table of Contents
	:maxdepth: 3
	
	code

******************
MATLAB <--> Python
******************

.. code-block:: matlab

	if command == 'matlab'
		command = 'python';
	end

.. code-block:: python

	if command == 'python':
		command = 'matlab'
		
Take a look at the code blocks above. One is in MATLAB and the other is in Python. Which one is which?

Python and MATLAB have very similar syntax so knowing one while learning the other can get tricky. It's  
easy to mix up the commands. 

A couple of resources are listed below to help users of both languages find
equivalent commands:

* MATLAB commands in numerical Python from Mathesaurus by Vidar Bronken Gundersen

	* `HTML <http://mathesaurus.sourceforge.net/matlab-numpy.html>`_
	* `PDF <http://mathesaurus.sourceforge.net/matlab-python-xref.pdf>`_
	
* `NumPy for Matlab users <https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html>`_ from SciPy.org

**************
Good Practices
**************

Good practices:
1. Format as you go. 
2. Comment wisely.
3. Short and simple. 
4. Write test cases (figure out when and how your code will fail).
5. Back it up. 

Debugging:
1. Know how to read error messages.
2. Don't just copy from online sources. 
3. Consult the documentation.
4. Diagnose with print statements.
5. Think first, then Google (figure out what you want your code to do then search for the corresponding functions).
	- Check if a function already exists for what you want to do. 
6. Use a debugger (breakpoint() after 3.7, pdb for before).

