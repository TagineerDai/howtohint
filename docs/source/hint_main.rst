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

Resources
^^^^^^^^^^^
2. `rst syntax <http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_ 
3. `publicate github page <https://blog.github.com/2016-08-22-publish-your-project-documentation-with-github-pages/>`_

Installation
^^^^^

Install Sphinx.  

>>> pip install sphinx sphinx-autobuild

Start ReadtheDocs project.

>>> mkdir docs && cd ./docs
>>> sphinx-quickstart

Edit content and real time test.  

If you use VS Code, `Live Server 
<https://ritwickdey.github.io/vscode-live-server/>`_ 
is highly recommended.

>>> cd ./source
>>> sphinx-autobuild . _build/html