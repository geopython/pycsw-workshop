pycsw-workshop
==============

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

Useful External References
--------------------------

* reStructuredText Reference Guide: http://docutils.sourceforge.net/docs/user/rst/quickref.html
* List of Python Packages: https://pypi.python.org/pypi?%3Aaction=index

License
-------

Copyright (c) 2013 pycsw Team

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
