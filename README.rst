MetPy
=====

.. image:: https://img.shields.io/pypi/l/metpy.svg
    :target: https://pypi.python.org/pypi/MetPy/
    :alt: License

.. image:: https://img.shields.io/github/issues/metpy/metpy.svg
    :target: http://www.github.com/metpy/MetPy/issues
    :alt: GitHub Issues

.. image:: https://img.shields.io/github/tag/metpy/metpy.svg
    :target: https://github.com/metpy/MetPy/tags
    :alt: GitHub Tags

.. image:: https://img.shields.io/pypi/v/metpy.svg
    :target: https://pypi.python.org/pypi/MetPy/
    :alt: Latest Version

.. image:: https://img.shields.io/pypi/dm/metpy.svg
    :target: https://pypi.python.org/pypi/MetPy/
    :alt: Downloads

.. image:: https://travis-ci.org/metpy/MetPy.svg?branch=master
    :target: https://travis-ci.org/metpy/MetPy
    :alt: Travis Build Status

.. image:: https://coveralls.io/repos/metpy/MetPy/badge.svg?branch=master
    :target: https://coveralls.io/r/metpy/MetPy
    :alt: Coveralls Coverage Status

.. image:: https://landscape.io/github/metpy/MetPy/master/landscape.svg?style=flat
    :target: https://landscape.io/github/metpy/MetPy/master
    :alt: Code Health

.. image:: https://readthedocs.org/projects/pip/badge/?version=latest
    :target: http://metpy.readthedocs.org/en/latest/
    :alt: Latest Doc Build Status

.. image:: https://readthedocs.org/projects/pip/badge/?version=stable
    :target: http://metpy.readthedocs.org/en/stable/
    :alt: Stable Doc Build Status

MetPy is a collection of tools in Python for reading, visualizing and
performing calculations with weather data.

MetPy is still in an early stage of development, and as such
**no APIs are considered stable.** While we won't break things
just for fun, many things may still change as we work through
design issues.

We support Python 2.7 as well as Python >= 3.2.

Important Links
---------------

- Source code repository: https://github.com/MetPy/MetPy
- HTML Documentation (stable release): http://metpy.readthedocs.org/en/stable/
- HTML Documentation (development): http://metpy.readthedocs.org/en/latest/
- Issue tracker: http://github.com/Metpy/MetPy/issues

Dependencies
------------
Other required packages:

- Numpy
- Scipy
- Matplotlib
- Pint

Philosophy
----------
The space MetPy aims for is GEMPAK (and maybe NCL)-like functionality, in a way that plugs easily
into the existing scientific Python ecosystem (numpy, scipy, matplotlib). So, if you take the average GEMPAK script
for a weather map, you need to:

- read data
- calculate a derived field
- show on a map/skew-T

One of the benefits hoped to achieve over GEMPAK is to make it easier to use these routines for any
meteorological Python application; this means making it easy to pull out the LCL calculation and just use that,
or re-use the Skew-T with your own data code. MetPy also prides itself on being well-documented and well-tested,
so that on-going maintenance is easily manageable.

The intended audience is that of GEMPAK: researchers, educators, and any one wanting to script up weather analysis.
It doesn't even have to be scripting; all python meteorology tools are hoped to be able to benefit from MetPy.
Conversely, it's hoped to be the meteorological equivalent of the audience of scipy/scikit-learn/skimage.