# doc
How to list in Read the Docs.

#### How to start a Read the Docs project?

```sh
# Install Sphinx.
pip install sphinx sphinx-autobuild
# Start project
mkdir docs && cd ./docs
sphinx-quickstart
# Edit content and real time test
cd ./source
sphinx-autobuild . _build/html
# Edit `.rst` files and refresh the build/index.html in your browser
```

#### How to publish the Read the Docs document on GitHub pages?

1. <https://read-the-docs.readthedocs.io/en/latest/getting_started.html#sign-up-and-connect-an-external-account>	
   1. Login to Read the Docs [dashboard](http://readthedocs.org/dashboard) with your GitHub account.
   2. Click import and choose the given repository.
2. 

