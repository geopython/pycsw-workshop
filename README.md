pycsw-workshop
==============

[![Build Status](https://travis-ci.org/geopython/pycsw-workshop.png?branch=master)](https://travis-ci.org/geopython/pycsw-workshop)

Background
----------

The initial pycsw workshop materials were created through funding provided by the 
[Oregon Coastal Management Program](http://www.oregon.gov/lcd/ocmp/Pages/index.aspx), 
through an FGDC CAP grant, in 2013.

Structure
---------

Workshop documentation is stored in reStructuredText.  HTML output is generated 
through the Sphinx documentation utility.

Installation
------------

### Using easy_install

*Note: the following steps assume that [Python](http://www.python.org/) and
Python's [setuptools package](https://pypi.python.org/pypi/setuptools) are installed 
and available in your PATH*

1. Install [Sphinx](http://sphinx-doc.org/)

     `easy_install Sphinx`
       
2. Install the [Bootstrap theme](https://github.com/ryan-roemer/sphinx-bootstrap-theme#installation) for Sphinx
 
     `easy_install sphinx_bootstrap_theme`

3. Install rst2pdf

     `easy_install rst2pdf`
     
4. Install the Python Imaging Library

     `easy_install pil`
     
   Note that you can optionally use the *pillow* library, which seems to work better on Ubuntu
       
5. Clone the pycsw repository locally

     `git clone git@github.com:geopython/pycsw-workshop.git pycsw-workshop`
     
### Using virtualenv / pip

You can also use [virtualenv](http://www.virtualenv.org/) and [pip](http://www.pip-installer.org/) as follows:

```

$ virtualenv venv
$ cd venv
$ git clone git@github.com:geopython/pycsw-workshop.git
$ cd pycsw-workshop
$ pip install -r requirements.txt

```

       
Generating HTML Output
----------------------

1. cd into *pycsw-workshop* directory

2. execute:

     `make html`
     
3. HTML output is in the *_build* directory

Generating PDF Output
---------------------

1. cd into *pycsw-workshop* directory

2. execute:

     `sphinx-build -b pdf . _build/html`
     
3. *pycsw-Workshop.pdf* should have been created in the *_build/html/* directory

Publishing to Live Site (Committers)
------------------------------------

To publish to the live site, simply run `make gh-pages`.

Contributions
-------------

Contributions, fixes, improvements and Pull Requests are always welcome.


Useful External References
--------------------------

* reStructuredText Reference Guide: http://docutils.sourceforge.net/docs/user/rst/quickref.html
* List of Python Packages: https://pypi.python.org/pypi?%3Aaction=index

