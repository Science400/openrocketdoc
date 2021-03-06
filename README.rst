===========================
Open Rocket Document Format
===========================

.. image:: https://img.shields.io/pypi/v/openrocketdoc.svg
        :target: https://pypi.python.org/pypi/openrocketdoc

.. image:: https://travis-ci.org/open-aerospace/openrocketdoc.svg?branch=master
    :target: https://travis-ci.org/open-aerospace/openrocketdoc

.. image:: https://coveralls.io/repos/github/open-aerospace/openrocketdoc/badge.svg?branch=master
        :target: https://coveralls.io/github/open-aerospace/openrocketdoc?branch=master

*Open Rocket Document* (.ord) is a suggested open document standard for
describing sounding rockets. Includes many useful format transformations for
use with scientific computing packages.


* Python 2 and 3 compatible
* Free software: GPLv3
* Full Documentation: https://open-aerospace.github.io/openrocketdoc.


Motivation
----------

There is no single tool that can do everything. This is true in many fields, and is true in aerospace as well. When it come to simulating rockets there are many packages and programs available. Often it's desirable to use many different ones and compare the results. Or it may be that one package only handles aerodynamics, and another makes a mass model. In fact this is quite common, and even desirable, as it lets one write code that does one thing, and one thing well.

The problem is these programs almost universally don't know how to communicate with each other. Sometimes this is intentional, for example certain proprietary programs, other times one program might be a holdover from the 1980's, and still use fixed with text file while anything modern would try and use something like JSON.

The relevant XKCD here is probably apt:

.. image:: https://imgs.xkcd.com/comics/standards.png

However I believe there are to date very few, perhaps none, existing universal standards for describing rockets.

Goals
-----

The goal is to create an extensible, universal, usable, interchangeable way of describing model and sounding rockets. I want to be able to both read and write to as many possible existing file types, and have a native file type for this project based on YAML (for human readability and to be version control system friendly).

This "Open Rocket Document" should be flexible enough to both roughly describe a preliminary design (say, this tall, this material) and detailed enough to fully describe a rocket that's been built and tested (aerodynamic tables, detail mass breakdown, etc.).

There should also be extensibility, for instance if you want to have your own tags on objects (that might be read and used by a custom program).

Often a single component (say, a certain fin construction) might be used on many different designs. So there is a strong desire to have the document optionally spread over many files. This would be at odds of a "Keep It Simple" approach however, so it remains to be seen how to implement.

Features
--------

* TODO
