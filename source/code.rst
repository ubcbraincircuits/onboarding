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

Learning how to code can be frustrating but it is ultimately rewarding. As a beginner, it is best to form good habits early.
Additionally, knowing common mistakes and some basic tricks can save a lot of time and effort. 

Format as you go
================

Sometimes when you're in the zone, the last thing you're worried about is your coding style. As a result, your code comes out looking like
a wild beast which is a nightmare to tame when it spits out errors.

Unformatted code is harder to debug because it's harder to read. It's therefore best if you format as you write. 

.. tip::
	In Python, code is good if it's *Pythonic* - see the section on :ref:`pycodestyle` for the specifics of Python style. Advanced coders can 
	take advantage of `Black <https://black.readthedocs.io/en/stable/installation_and_usage.html#installation>`_, a Python formatter.
	
	MATLAB does not have an official style guide. However, there is a popular document called `MATLAB Style Guideline 2.0 <https://www.mathworks.com/matlabcentral/fileexchange/46056-matlab-style-guidelines-2-0>`_
	written by Richard Johnson for those interested in polishing up their code. 

Comment wisely
==============

Comments are essential because they describe the purpose of your code. It's important to write code that future you and other people will undestand.
For example, functions should always be accompanied by a description.

It's good to comment frequently but do so with some discretion - try not to comment the obvious. 

.. hint::
	Comments begin with a ``#`` in Python and a ``%`` in MATLAB. 

Don't just copy from online sources
===================================

It's easy to stitch together a script from code snippets you find online but it's not a productive learning experience. 
A valuable part of learning how to code is problem-solving, so it pays off to figure it out on your own first. 

If you're really stuck and need help, at least try to understand what each line of code does before using it. 

Write test cases: Catch me if you can!
======================================

Back it up
==========

*********
Debugging
*********

	"90% of coding is debugging. The other 10% is writing bugs"
	-- `@bramcohen <https://twitter.com/bramcohen/status/51714087842877440>`_
	
There is a good reason why this tweet has thousands of retweets and likes - because 
it's sometimes true. Here are some tips when expectation ``!=`` reality when coding. 

Consult the documentation
=========================

Debugging can be as easy as checking the documentation. When the output of your code doesn't make
sense, it might be because:

- a command you're using does not do what you think it does 
- you're not providing the correct input argument(s) to a command
- you forgot to specify a value for a default argument of a command 

For all these cases, reading the documentation carefully will likely resolve the issue. 

.. attention::
	Before writing your own function, check if a command already exists for the result you require!

Learn to read and write error messages
======================================

Diagnose with print statements
==============================

One of the simplest ways to find out where your code is going wrong is to insert print statements between lines.

.. admonition:: Example
	
	.. highlight:: python
	
	::
		
		>>> for item in some_range:
		...:	# insert step 1 here
		...:	print("Step 1 complete!")
		...:	# insert step 2 here 
		...: 	print("Step 2 complete!")
	
	When you run the for loop, you'll know exactly where the bug occurs by which print statement fails to appear. 
		 
Think first, then Google
========================

It's tempting to Google an error straightaway but this prevents you from building an intuition for debugging. 
Spend some time thinking about the logic of your code first; often times, there is a disparity between what you want your computer to do and what it is actually doing. 

Doing this will familiarize you with solutions to errors that may pop up again in the future and it may even help you foresee the same errors before you hit :guilabel:`Run`.
     
Use a debugger
==============

1. Know how to read error messages.
2. Don't just copy from online sources. 
3. Consult the documentation.
4. Diagnose with print statements.
5. Think first, then Google (figure out what you want your code to do then search for the corresponding functions).
	- Check if a function already exists for what you want to do. 
6. Use a debugger (breakpoint() after 3.7, pdb for before).

