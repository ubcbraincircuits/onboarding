##########################
Beginner's Guide to Coding
##########################

.. contents:: Table of Contents
	:depth: 3
	
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
	In Python, *Pythonic* code is good code - see the section on :ref:`pycodestyle <pycodestyle>` for the specifics of Python style. Advanced coders can 
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

In programming, it is best to be proactive - know when and how your code will fail. Run test cases through your functions to 
ensure that they give the expected result in every scenario. 

This is especially important if the code you are producing will be used by others so you can catch the errors and prevent your
program from crashing on users.

.. attention::
	Don't forget to address the edge cases! 

Back it up
==========

Coding takes a lot of work so you don't want to lose your progress when your program crashes. This lesson is painful to learn by mistake so 
back up your code regularly or better yet, version it! 

See the section on :ref:`version-control` in the Data Management Page. 

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

As with everything else in life, coding requires you to learn from your mistakes but before you can learn from them, 
you must first know exactly what those mistakes are and what caused them.

Errors can be more puzzling than the code that caused them. However, often times, they are actually
helpful and descriptive - that is, if you know how to read them. It takes practice but with time and experience,
you'll have an inkling about what's wrong with your code even with the vaguest of error messages.

Before you start coding, take some time to read up on the documentation about error handling. 

 - `Errors and Exceptions <https://docs.python.org/3.7/tutorial/errors.html>`_ in Python
 - `Error Handling <https://www.mathworks.com/help/matlab/error-handling.html>`_ in MATLAB
 
Knowing how to read error messages will also help you once you start writing your own programs. To make sure your programs
are user-friendly, make sure you anticipate potential mistakes your users may make so you can write clear error messages to
help them (remember :ref:`this<Write test cases: Catch me if you can!>` good practice?).
		
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
	
	When you run the for loop, you'll know exactly if and where a bug occurs by which print statement fails to appear. 
	
.. tip::
	Python has a standard `logging <https://docs.python.org/3/library/logging.html>`_ module, which can track events while
	a program runs. Logging can be used to check and record the execution of your code, including errors and warnings. This is a more 
	robust and efficient approach to debugging than print statements. 
	
	.. highlight
	
	::
	
		>>> import logging
		 
Think first, then Google
========================

It's tempting to Google an error straightaway but this prevents you from building an intuition for debugging. 
Spend some time thinking about the logic of your code first; often times, there is a disparity between what you want your computer to do and what it is actually doing. 

Doing this will familiarize you with solutions to errors that may pop up again in the future and it may even help you foresee the same errors before you hit :guilabel:`Run`.
     
Use a debugger
==============

A debugger should only be your last line of defense. For beginners, it is better to establish your ability to diagnose problems before
relying on a debugger. 
	
The Python Debugger (pdb)
-------------------------

`pdb <https://docs.python.org/3/library/pdb.html>`_ is a module from the Python Standard Library that interactively debugs Python programs.
This module enables coders to step through their programs line-by-line as it executes.

	- `How To Use the Python Debugger <https://www.digitalocean.com/community/tutorials/how-to-use-the-python-debugger>`_, a tutorial
	  that highlights the features of pdb written by Lisa Tagliaferri for DigitalOcean
	- `pdb Tutorial <https://github.com/spiside/pdb-tutorial>`_, a tutorial that uses an example of a Python script for a dice game to illustrate the use of pdb.

.. note:: 
	A **breakpoint** is used to pause a running program at a specific location and *break* into the debugger, allowing 
	you to step through the code following the breakpoint. 
	
	In Python, a breakpoint can be hard-coded into a program by first importing the pdb module then inserting the breakpoint method 
	above the line at which you would like the debugging session to begin. 
	
	.. code-block:: python
	
		import pdb
		# some code in between
		pdb.set_trace()
		# debugger begins at this line
		
.. tip::
	For versions 3.7 and onwards, a built-in ``breakpoint()`` function can replace ``import pdb; pdb.set_trace()``.
	
Debugging in MATLAB
-------------------

MATLAB automatically generates warnings for lines that may cause errors. These warnings are indicated by orange
highlight within the script and as orange lines in a narrow sidebar on the right-hand side of the Editor. 

Debugging in MATLAB can be done in one of two ways:

	1. point-and-click through the Editor/Debugger: `Debug a MATLAB Program <https://www.mathworks.com/help/matlab/matlab_prog/debugging-process-and-features.html>`_
	2. through debugging functions in the Command Window: `Debugging and Analysis <https://www.mathworks.com/help/matlab/debugging-code.html?s_tid=CRUX_lftnav>`_
		
.. tip::
	In MATLAB, ``dbstop`` is the equivalent function to ``breakpoint()`` in Python. 

