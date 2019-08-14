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

UC Berkeley offers a course called `Applied Statistics for Neuroscientists <https://github.com/charlesfrye/AppliedStatisticsForNeuroscience>`_.

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
	
.. attention::

	Before you start Part 02-10: Model Fitting, open utils.py in the util folder and comment out all instances of ``ax.set_aspect('equal')``. This command
	does not apply to 3D plots and will therefore prevent them from rendering. 
	
	An equivalent function called ``axis_equal_3d`` was included instead,
	which was written by Stack Overflow user Ben as a response to this `post <https://stackoverflow.com/questions/8130823/set-matplotlib-3d-plot-aspect-ratio/19933125>`_.
	
	
