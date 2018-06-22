.. Hint by Tagineer documentation master file, created by
   sphinx-quickstart on Thu Jun 21 14:28:03 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Hint by Tagineer
===================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

.. Indices and tables
=====================

.. * :ref:`1.1`

How to use Read the Docs?
---------------------------

1. `rst syntax <http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_ 
2. `publicate github page <https://blog.github.com/2016-08-22-publish-your-project-documentation-with-github-pages/>`_

Install Sphinx.  

>>> pip3 install sphinx sphinx-autobuild

Start ReadtheDocs project.

>>> mkdir docs && cd ./docs
>>> sphinx-quickstart

Edit content and real time test.  

If you use VS Code, `Live Server 
<https://ritwickdey.github.io/vscode-live-server/>`_ 
is highly recommended.

>>> cd ./source
>>> sphinx-autobuild . _build/html

How to deep copy?
------------------------

>>> in python 
import copy
different_obj = copy.deepcopy(current_obj)

How to insert equation?
---------------------------

In Picture
^^^^^^^^^^^^
1. `PNG by MathURL <http://mathurl.com/>`_
2. `GIF by EqnEditor <http://www.codecogs.com/latex/eqneditor.php>`_

In HTML 
^^^^^^^^^
1. Setting globally. 

Add the following line in your home page, 
and insert latex equation with ``$``.

>>> in HTML
<script type="text/javascript" 
src="http://common.cnblogs.com/script/ASCIIMathML.js">
</script>

2. Use just once.

Insert with ``YOUR_LaTeX_CODE`` replaced by 
your LaTeX equation.

>>> in HTML
<img src="http://latex.codecogs.com/gif.latex?YOUR_LaTeX_CODE" />