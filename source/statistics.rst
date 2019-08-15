##########
Statistics
##########

Statistics is an inevitable part of research but not necessarily an inevitable or significant part of undergraduate education. 

Since neuroscientists come from a diverse range of backgrounds, knowledge and understanding of statistics can vary greatly 
from person to person so here are some resources on statistics in neuroscience flavor. 

.. contents:: Table of Contents
	:depth: 3

*************************************************
Applied Statistics for Neuroscience (UC Berkeley)
*************************************************

The materials for a UC Berkeley course called `Applied Statistics for Neuroscientists <https://github.com/charlesfrye/AppliedStatisticsForNeuroscience>`_
are available on GitHub. The course is an intensive introduction to statistics and provides an opportunity to gain a solid understanding
of frequently used statistical methods in neuroscience which are not always explained in depth.

The course constitutes of tutorials and labs in Jupyter notebooks, which are organized into three parts:

**Part 00: Setup and Review**

	- 00 - Setup
	- 01 - Probability and Statistics Review
	
		- Lab A - Probability and Python
		- Lab B - Statistics with Pandas and Seaborn
		
**Part 01: Statistical Testing**

	- 02 - Inferential Statistics and Error Bars 
	
		- Lab A - Inferential Statistics
		- Lab B - Error Bars 
	
	- 03 - Hypothesis Testing
	
		- Tutorial - Hypothesis Testing
		- Lab - Hypothesis Testing
		
	- 04 - Tests for 2-Sample Data
	
		- Tutorial - Tests for 2-Sample Data
		- Lab A - Unpaired t-tests
		- Lab B - Paired t-tests and Non-Parametric Tests 
		
	- 05 - ANOVA I
		
		- Tutorial - ANOVA by Hand
		- Lab - One-Way ANOVA
		
	- 06 - ANOVA II
	
		- Tutorial - Two-Way Anove by Hand
		- Lab A - Two-Way ANOVA
		- Lab B - Multiple Comparisons and ANOVA
		
**Part 02: Statistical Modeling**

	- 07 - Linear Algebra
	
		- Tutorial - Linear Algebra for Neuroscientists
		- Lab - Linear Transformations
		
	- 08 - Bootstraping and Correlation
	
		- Tutorial A - Sampling and Bootstrapping
		- Lab A - Visualizing Bootstrapping and One-Sample Tests
		- Tutorial B - Dependence and Correlation
		- Lab B - Computing and Bootstrapping Correlation 
		
	- 09 - Model Specification 
	
		- Lab - Visualizing Models
		
	- 10 - Model Fitting 
	
		- Lab -Fitting Models
		
	- 11 - Model Accuracy and Reliability 
		
		- Lab - Model Accuracy and Reliability
		
	- 12 - Classification
	
		- Lab - Classification
		
	- 13 - Clustering
	
		- Tutorial - Clustering 

Since the code used for examples is written in Python, familiarity with the language would be helpful and is therefore recommended.

.. attention::

	To prevent errors while running the notebooks, ensure the latest versions of matplotlib and seaborn are installed on your computer. Enter the command 
	
	.. code-block:: console
	
		$ pip install --upgrade --user matplotlib 
		
	into Terminal or Command Prompt. 
	
.. error::

	Before you start Part 02-10: Model Fitting, open utils.py in the util folder and comment out all instances of ``ax.set_aspect('equal')``. This command
	does not apply to 3D plots and will therefore prevent them from rendering. 
	
	An equivalent function called ``axis_equal_3d`` was included instead,
	which was written by Stack Overflow user Ben as a response to this `post <https://stackoverflow.com/questions/8130823/set-matplotlib-3d-plot-aspect-ratio/19933125>`_.

*****************************************************************************
Statistics and Data Analysis Tutorial (Center for Brains, Minds and Machines)
*****************************************************************************	
	

The `Brains, Minds and Machines (BMM) Summer Course <https://cbmm.mit.edu/summer-school>`_ by `The Center for Brains, Minds and Machines (CBMM) <https://cbmm.mit.edu/>`_ 
at MIT is a three-week course on computation, neuroscience, and cognition in the fields of human and machine intelligence research. 

The `Statistics and Data Analysis tutorial <https://www.youtube.com/watch?v=XbHeCL_8UhA&>`_ from the 2018 BMM summer course is available on Youtube.
It is a quick overview of the basics of statistics by Ethan Meyers.

:00\:\00-10\:\13: `Introduction <https://www.youtube.com/watch?v=XbHeCL_8UhA&>`_
:10\:\14-12\:\22: `Box and violin plots <https://youtu.be/XbHeCL_8UhA?t=614>`_
:12\:\23-13\:\42: `Joy plots <https://youtu.be/XbHeCL_8UhA?t=743>`_
:13\:\43-14\:\52: `Dynamite plots <https://youtu.be/XbHeCL_8UhA?t=823>`_
:14\:\53-16\:\40: `What is a statistic? <https://youtu.be/XbHeCL_8UhA?t=893>`_
:16\:\41-18\:\26: `Correlation coefficient <https://youtu.be/XbHeCL_8UhA?t=1001>`_
:18\:\27-19\:\22: `Descriptive statistics <https://youtu.be/XbHeCL_8UhA?t=1107>`_
:19\:\23-19\:\48: `Population/process parameters <https://youtu.be/XbHeCL_8UhA?t=1163>`_
:19\:\49_-20\:\11: `Statistical Inference <https://youtu.be/XbHeCL_8UhA?t=1189>`_
:20\:\12-20\:\24: `Estimation <https://youtu.be/XbHeCL_8UhA?t=1212>`_
:20\:\25-22\:\27: `Regression <https://youtu.be/XbHeCL_8UhA?t=1225>`_
:22\:\28-23\:\56: `Sampling Distribution <https://youtu.be/XbHeCL_8UhA?t=1348>`_
:23\:\57-24\:\29: `Estimation (continued) <https://youtu.be/XbHeCL_8UhA?t=1437>`_
:24\:\30-27\:\17: `Confidence intervals <https://youtu.be/XbHeCL_8UhA?t=1470>`_
:27\:\18-33\:\17: `Bootstrapping, 95% confidence interval <https://youtu.be/XbHeCL_8UhA?t=1638>`_
:33\:\18-35\:\05: `What is a p-value? <https://youtu.be/XbHeCL_8UhA?t=1998>`_
:35\:\06-40\:\34: `Hypothesis testing <https://youtu.be/XbHeCL_8UhA?t=2106>`_
:40\:\35-41\:\34: `Permutation tests, parametric tests <https://youtu.be/XbHeCL_8UhA?t=2435>`_
:41\:\35-43\:\29: `Visual hypothesis tests <https://youtu.be/XbHeCL_8UhA?t=2495>`_
:43\:\30-53\:\50: `Permutation test example <https://youtu.be/XbHeCL_8UhA?t=2610>`_
:53\:\51-58\:\28: `Type I and Type II errors <https://youtu.be/XbHeCL_8UhA?t=3231>`_
:58\:\29-1\:\03\:\44: `Multiple hypothesis tests <https://youtu.be/XbHeCL_8UhA?t=3509>`_
:1\:\03\:\45-end: `Data Science <https://youtu.be/XbHeCL_8UhA?t=3825>`_

