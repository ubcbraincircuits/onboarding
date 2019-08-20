###############
Data Management
###############

With big data comes big responsibility.

.. contents:: Table of Contents
	:depth: 3
	
*****************
Data Repositories
*****************

Scholars Portal Dataverse
=========================

`Scholars Portal Dataverse <https://dataverse.org/>`_ is a research data repository that emphasizes discoverability and long-term preservation
of data while ensuring academic credit. For more information, see the section on Scholars Portal Dataverse in the UBC Brain Circuits Data Management white paper.

The Brain Circuits Cluster has its own `dataverse <https://dataverse.scholarsportal.info/dataverse/UBC_BrainCircuits>`_,
within which certain labs have set up their own dataverses.

.. attention::
	The maximum file size for upload on Scholars Portal Dataverse is 2.5 GB.

If a dataverse for your lab already exists, ask your PI for access.

If your lab is interested in creating a dataverse, contact Jeffrey LeDue through email (jledue@mail.ubc.ca).

Federated Research Data Repository (FRDR)
=========================================

The `Federated Research Data Repository (FRDR) <https://www.frdr.ca/repo/?locale=en>`_ is a collaboration between Portage,
Compute Canada (CC), and the Canadian Association of Research Libraries (CARL) which provides a system that combines
curated large-scale data preservation with data discovery across Canadian research data repositories. Refer to the FRDR section
in the UBC Brain Circuit's Data Management white paper for more information.

Datasets in FRDR are searchable by anyone, however FRDR is currently in Limited Production and therefore only accepts
data deposits from a select number of research groups. The cluster is pleased to be the first in Canada and in UBC to 
deposit a dataset into FRDR.

PIs can deposit datasets into the `cluster's FRDR collection <https://www.frdr.ca/repo/handle/ubcbraincircuits>`_ by becoming
a depositor. Contact Jeffrey LeDue (jledue@mail.ubc.ca) to request access.

.. attention::
	FRDR automaticallly archives data submissions less than 4 TB. 


.. _version-control:
	
***************
Version Control
***************

Simply put, version control is a way of tracking changes to a file. 
It can seem like a lot of work on top of the big helping of work you likely already have 
so why add it to your plate?

Version control is the solution to many problems which are unfortunately familiar:

	- **File recovery**: computer crash, accidental deletion, corrupted file - in case of emergency, break the version control glass. 
	
	- **Versioning**: Make experimental changes without relying on the undo button to save you when things goes awry. 
	
	- **Backup**: Lost your copy of the file? Working from another computer? No problem. 
	
	- **Attribution**: Credit is given where credit is due. A record of user contributions simplifies collaboration.
	
	- **Changelog**: Have you ever looked at previous work and wondered, *Why did I do that?*? Version control keeps a record of the changes you've made and why you've made them so your past self doesn't confuse your future self. 
	
.. note::
	A **remote** repository is hosted on a server (online) while a **local** repository exists on a computer (offline). When referring to the same
	repository, the local *repo* is usually a clone of the remote which typically lives on GitHub.
	
Git
===

`Git <https://git-scm.com/>`_ is a popular open-source distributed version control system. 

`GitHub <https://github.com/>`_ hosts Git repositories. Check out the cluster's `GitHub Team repository <https://github.com/ubcbraincircuits>`_.
Each lab can be added as a Team. If interested, please contact Jeffrey LeDue (jledue@mail.ubc.ca).

.. tip::
	Learning Git can be a tough task. Here are some resources to help you get started:
	
		- `Git Handbook <https://guides.github.com/introduction/git-handbook/>`_, a 10-minute read on the basics of Git and its integration with GitHub
		- `An introduction to Git: what it is, and how to use it <https://www.freecodecamp.org/news/what-is-git-and-how-to-use-it-c341b049ae61/>`_, a tutorial on Git commands by freeCodeCamp 