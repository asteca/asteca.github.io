Input data files
================

There are two types of required input files: the ``asteca.ini`` general input
parameters file, and the file that contains the cluster data.

The former contains the parameters used to run all the functions included within
**ASteCA**; it is included with the package.

The latter is provided by the user and it needs to be formatted such that it can
be loaded by the `pandas.read_csv()
<https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html>`_
module. This file must be stored in the ``input/`` folder and its
associated plots and output files will be stored in the ``output/`` folder.
All the files inside the ``input/`` folder (inside or outside a
sub-folder) will be processed by **ASteCA**.


Theoretical isochrones
----------------------

**ASteCA** needs at least one set of theoretical isochrones stored in the
``isochrones/`` folder, to be able to apply the *best-fit* function that
estimates the clusters’ parameters.
Currently, the only isochrone files supported are those obtained via the
`CMD service`_ (`Girardi et al. 2002`_), but any set can in theory be used
(with some changes made to the code).
Please `contact me <gabrielperren@gmail.com>`_ if you wish to use a different
set of theoretical isochrones.

The isochrones must be downloaded with the package `ezPadova-2`_.
This code takes care of downloading the isochrones for a given range of
metallicities, storing them in files named following the proper
naming convention, and place them inside a folder also with the correct name.

This way, once this code finishes you can just cut the generated folder and
paste it inside the ``isochrones/`` folder in **ASteCA**.


.. _CMD service: http://stev.oapd.inaf.it/cgi-bin/cmd
.. _Girardi et al. 2002: http://www.aanda.org/articles/aa/abs/2002/31/aah3268/aah3268.html
.. _ezPadova-2: https://github.com/asteca/ezpadova-2
