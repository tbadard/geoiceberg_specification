# GeoIceberg specification

GeoIceberg specification details how to add support for a geometric data type in Apache Iceberg to store geospatial data in an Iceberg table.

This specification and its translations are released under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

This repository holds the source files of the https://geoiceberg.org website. The later is propeled by the [mkdocs](https://www.mkdocs.org/) tool.

## Build the website

To build the website, you have to install the mkdocs tool and plugins for internationalization first.

MkDocs requires a recent version of [Python] and the Python package manager, [pip], to be installed on your system.

You can check if you already have these installed from the command line:

```console
$ python3 --version
Python 3.8.2
$ pip --version
pip 20.0.2 from /usr/local/lib/python3.8/site-packages/pip (python 3.8)
``
Create a virtual environment dedicated to mkdocs

```console
$ python3 -m venv mkdocs
$ source mkdocs/bin/activate
``

Then, install the mkdocs tool and required plugins

```console
$ python3 -m pip install 'mkdocs[i18n]'
$ python3 -m pip install mkdocs-i18n
``

Finally, the website is created with:

```console
$ mkdocs build 
``

If you want to preview the website locally while you are editing the markdown source files

```console
$ mkdocs serve 
``

