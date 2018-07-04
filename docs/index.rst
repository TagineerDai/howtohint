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



How to use Read the Docs?
---------------------------

1. `rst syntax <http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_ 
2. `publicate github page <https://blog.github.com/2016-08-22-publish-your-project-documentation-with-github-pages/>`_

Install Sphinx.  

>>> pip3 install sphinx sphinx-autobuild sphinx_rtd_theme

Start ReadtheDocs project.

>>> mkdir docs && cd ./docs
>>> sphinx-quickstart

Edit content and real time test. 

In your `conf.py`, change `html_theme` to `html_theme = "sphinx_rtd_theme"`.

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

How to release a port?
------------------------

>>> Only one usage of each socket address is normally permitted.

Windows
^^^^^^^^

Find process using this port.

>>> netstat -ano|findstr <PORT_NUMBER>
# 172 is the PID of the process
TCP    127.0.0.1:8001         0.0.0.0:0              LISTENING       172

Kill the process.

>>> tskill 172

Linux
^^^^^

>>> sudo kill $(sudo lsof -t -i:<PORT_NUMBER>)

To Force the command:

>>> sudo kill -9 $(sudo lsof -t -i:9001)

Or the same as for NT system:

>>> sudo netstat -lpn |grep :<PORT_NUMBER>
# 93711 is the process id.
tcp     0   0 127.0.0.1:8888    0.0.0.0:*   LISTEN      93711/python3
# Kill the process by pid or pname.
kill 6782

How to Use Docker?
---------------------

Build your customized workdir.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

>>> cd into the dir where Dockerfile lives.
Docker build -t <image_name>.
docker image rm <image_name>/<image_id>
docker login # with your docker hub username and passwd
docker push <image_name>


How to setup ``librosa`` env?
-----------------------------

>>> pip3 install librosa
sudo apt-get install linuxbrew-wrapper 

How to solve the ``no backend error`` caused by ``audioread``? 

Accroding to `the discussion <https://groups.google.com/forum/#!topic/librosa/Z1-HXBsHLi0/discussion>`_, we should install `audioread <https://github.com/beetbox/audioread>`_'s backends.

Let's try ``ffmpeg``:

>>> sudo add-apt-repository ppa:djcj/hybrid -y
sudo apt-get update  
sudo apt-get install ffmpeg -y

>>> # for scikits.samplerate
sudo apt-get install libsamplerate0 libsamplerate0-dev
pip install scikits.samplerate

>>> sudo apt-get install linuxbrew-wrapper 
brew install libsamplerate

Downloaded music from http://www.brainybetty.com/soundsforpowerpoint2.htm.