<img src=https://github.com/raoulcollenteur/pydrus/blob/master/docs/_static/logo.png width=120, align=left>

# Pydrus: Python implementation of HYDRUS-1D

<a href="http://www.gnu.org/licenses/gpl-3.0.txt"><img src=https://img.shields.io/github/license/raoulcollenteur/pydrus> </a>
<a href="https://pypi.python.org/pypi/pydrus"> <img src=https://img.shields.io/pypi/pyversions/pydrus> </a>
<a href="https://github.com/pastas/pydrus/releases"> <img src=https://img.shields.io/github/release-pre/raoulcollenteur/pydrus> </a>
<a href="https://pydrus.readthedocs.io/en/latest/?badge=latest"> <img src="https://readthedocs.org/projects/pydrus/badge/?version=latest"></a>
[![Build Status](https://travis-ci.org/raoulcollenteur/pydrus.svg?branch=master)](https://travis-ci.org/raoulcollenteur/pydrus)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/2560d404fb8540e0acb847fefe30a301)](https://www.codacy.com/app/pastas/pydrus?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=raoulcollenteur/pydrus&amp;utm_campaign=Badge_Grade)
[![codecov](https://codecov.io/gh/raoulcollenteur/pydrus/branch/master/graph/badge.svg)](https://codecov.io/gh/raoulcollenteur/pydrus)

This package provides a Python implementation of the HYDRUS-1D unsaturated zone model developed by Šimůnek, J., M. Th. van Genuchten, and M. Šejna. More information on the HYDRUS-1D model is available [here](https://www.pc-progress.com/en/Default.aspx?hydrus-1d). This software is licenced under the GNU GENERAL PUBLIC LICENSE found [here](http://www.gnu.org/licenses/gpl-3.0.txt). The Pydrus code is developed by R.A. Collenteur, G. Brunetti and M. Vremec. With Pydrus, a HYDRUS-1D model can be created, calibrated and visualized through Python scripts, making it easy to adjust the model and providing a 100% reproducible workflow of your modeling process.

## Examples and Documentation
Examples of using Pydrus can be found in the example folder. This folder also contains a number of Jupyter Notebooks that thoroughly explain the use of the software. Documentation is still under development.

## Installing Pydrus
### 1. Installing the Python package
The Pydrus package will be available on the Pypi package index as the software moves towards production ready software. To install in developer mode, use the following syntax:

`>>> pip install -e .`

### 2. Compiling the source code
Before you can use Pydrus the adapted Fortran77 files need to be compiled to an executable. The makefile (MacOS/Linux) and the make.bat (Windows) in the `source` folder are available to create the hydrus executable. Move into the source folder (which you can download from this GitHub page) and use the following syntax in your terminal or windows command line to compile the source code:
 
`>>> make`
 
This should create a Windows or Linux Executable that can be used to run the HYDRUS-1D simulation. In the Python code, you have to reference to the location of the executable so you can store it anywhere you want.
 
## Developing Pydrus
Pydrus is a community effort and help is always welcome. If you have found abug, please open a GitHub issue to report it. Pull requests including bug fixes and new functionality are very welcome and will be accepted on the Dev-branch of this repository.

## Citing Pydrus
If you use pydrus for one of your projects, we ask that you cite the code as follows:
*Collenteur, R.A., Brunetti, G., and M. Vremec (2019) Pydrus: Python implementation of the HYDRUS-1D unsaturated zone model. Version X.X.X* 
