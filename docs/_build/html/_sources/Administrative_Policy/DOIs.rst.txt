.. role:: raw-html-m2r(raw)
   :format: html


Implementing Read the docs
==========================

Tutorials
---------


* `Getting started with sphinx <https://docs.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html>`_
* `General tutorial <https://www.youtube.com/watch?v=hM4I58TA72g&t=2665s>`_
* `Read the docs tutorial <https://sphinx-tutorial.readthedocs.io/>`_ - Good!  

Preparation: Installing environments
------------------------------------

`Tutorial <https://www.youtube.com/watch?v=O5-zaf2Kcus>`_\ :


* 
  Anaconda: library that contains both python and packages (like sphinx)

* 
  Git: command line tool for version control

* 
  MS Visual Studio Code: a code Editor

* 
  Check if installs is ok:  

* 
  Open command prompt and type:  


  * 
    conda --version  

  * 
    git --version  

if you get "git is not a recognised command", the programs have not been installed properly.

add both conda and python to your path: https://www.datacamp.com/community/tutorials/installing-anaconda-windows

Test set-up for git, bash and anaconda: 
https://www.earthdatascience.org/workshops/setup-earth-analytics-python/setup-git-bash-anaconda/
Search for and open the Git Bash program. In this Terminal window, type bash and hit enter. If you do not get a message back, then Bash is available for use.

Next, type git and hit enter. If you see a list of commands that you can execute, then Git has been installed correctly.

Next, type conda and hit enter. Again, if you see a list of commands that you can execute, then Anaconda Python has been installed correctly.

Close the Terminal by typing exit.

Install anaconda for **linux subsystem windows**\ :  


* 
  https://medium.com/hugo-ferreiras-blog/using-windows-subsystem-for-linux-for-data-science-9a8e68d7610c  

* 
  https://gist.github.com/kauffmanes/5e74916617f9993bc3479f401dfec7da

local Windows hard drives are accessible at the following paths in Bash:\ :raw-html-m2r:`<br>`
cd /mnt/e/username/folder1/folder2

Using Git with VS Code
^^^^^^^^^^^^^^^^^^^^^^

`Tutorial <https://www.youtube.com/watch?v=9cMWR-EGFuY&t=19s>`_\ :raw-html-m2r:`<br>`
Copy URl of Github repository: Open using ctrl+shf+p
git: clone  

Set up Visual Studio Code as python IDE:
On Windows, make sure the location of your Python interpreter is included in your PATH environment variable. You can check this by running path at the command prompt. If the Python interpreter's folder isn't included, open Windows Settings, search for "environment", select Edit environment variables for your account, then edit the Path variable to include that folder.
Open Anaconda prompt
Type where python

Read The Docs: General workflow
-------------------------------

.. list-table::
   :header-rows: 1

   * - reStructuredText
     - Docutils
     - Sphinx
     - ReadTheDocs
   * - Markup language
     - python implementation of rst
     - wrapper for documentation tools
     - hosts sphinx project - publicly available
   * - lh
     - 
     - 


Github Repository Structure
^^^^^^^^^^^^^^^^^^^^^^^^^^^

ReadTheDocs (repo)  

..

   |-Readme.md\ :raw-html-m2r:`<br>`
   |-docs  

   ..

      |- **index.rst** : toctree (table of contents), index file fort the documentation\ :raw-html-m2r:`<br>`
      |- conf.py : Customisation of Sphinks\ :raw-html-m2r:`<br>`
      |- *Makefile* : Interface local development, do not touch\ :raw-html-m2r:`<br>`
      |- *make.bat* : Interface local development, do not touch\ :raw-html-m2r:`<br>`
      |- _build : output files go in here\ :raw-html-m2r:`<br>`
      |- _static : include statice files like images\ :raw-html-m2r:`<br>`
      |- _templates : Override Sphinx templates to customise look and feel\ :raw-html-m2r:`<br>`
      |- **index.rst**  : Own documentation\ :raw-html-m2r:`<br>`
      |- **support.rst**  : Own documentation\ :raw-html-m2r:`<br>`
      |- **something_else.rst**  : Own documentation  


What files to we want to put in there?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Check CoreTrustSeal documentation
