
.. ASteCA documentation master file, created by
   sphinx-quickstart on Thu Sep 18 11:26:27 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. image:: _static/asteca_icon.png
   :align: center

ASteCA
======

.. warning::
   This documentation is updated as the package evolves and it is possibly
   outdated and/or incomplete. Feel free to `contact me`_ if you have questions
   about using **ASteCA** in your research, or `open a new issue`_ in the
   code's repository.

This is the manual of operation for the Automated Stellar
Cluster Analysis (**ASteCA**) package.
**ASteCA** is an open source code developed entirely in Python, designed to
handle the usual tests applied to stellar clusters in order to
determine their characteristics: center, radius, membership probabilities
and associated intrinsic/extrinsic parameters (metallicity, age, extinction,
distance, binarity, total mass, etc).

The code is currently designed as a large script that combines functions
sequentially. This allows the user to select which ones to run and which to
skip, through a single input data file.


.. _contact me: mailto:gabrielperren@gmail.com
.. _open a new issue: https://github.com/Gabriel-p/asteca/issues/new



.. toctree::
   :maxdepth: 2
   :caption: User Guide

   install
   input_data
   running
   best_fit



License & Attribution
---------------------

Copyright 2015-2022 Gabriel I Perren.

**ASteCA** is free software made available under the GPL3 License. For details
see the `LICENSE`_.

The accompanying article describing the code in detail can be accessed
via `A&A <http://www.aanda.org/articles/aa/abs/2015/04/aa24946-14/aa24946-14.html>`_,
and referenced using the following BibTeX entry:

.. code-block:: Bibtex

   @article{Perren_2015,
       author = {{Perren, G. I.} and {V\'azquez, R. A.} and {Piatti, A. E.}},
       title = {ASteCA: Automated Stellar Cluster Analysis},
       DOI= "10.1051/0004-6361/201424946",
       url= "http://dx.doi.org/10.1051/0004-6361/201424946",
       journal = {A\&A},
       year = 2015,
       volume = 576,
       pages = "A6",
       month = "04",
   }


.. _LICENSE: https://github.com/asteca/ASteCA/blob/master/LICENSE.txt


Changelog
---------

.. include:: CHANGELOG.rst