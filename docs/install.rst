.. _sect-requirements:

Installation
============

The code has been tested with the latest release of `Python`_ available at the
time (3.9.12). The following packages are required to run **ASteCA**:
`pandas`_, `astropy`_, `sciPy`_, `numpy`_, `matplotlib`_, and `ptemcee`_.
The `emcee`_ and `corner.py`_ packages are optional, although some functions
and plots will not work without them.


.. _Python: https://www.python.org/downloads/
.. _pandas: https://pandas.pydata.org/
.. _astropy: http://www.astropy.org/
.. _sciPy: http://www.scipy.org/
.. _numpy: http://www.numpy.org/
.. _matplotlib: http://matplotlib.org/
.. _ptemcee: https://github.com/willvousden/ptemcee
.. _emcee: https://github.com/dfm/emcee/
.. _corner.py: https://corner.readthedocs.io/en/latest/



.. _sect-anaconda:

Working environment
-------------------

We use the `conda`_ package and environment manager to install all the necessary
dependencies to run **ASteCA** in an isolated Python environment. To install
conda,  follow these steps:

1. Go to https://conda.io/miniconda.html and download the appropriate version
   for your system. I recommend using the **Python 3.x** version and will assume
   in what follows that you are running a 64 bit Linux system.
2. Install with 

   .. code-block:: bash

     $ bash Miniconda3-latest-Linux-x86_64.sh

   Select yes when asked: *Do you whish the installer to prepend the Miniconda3
   install location to PATH in your ~/path?*
3. Close and re-open your terminal window for the changes to take effect. Move
   inside the directory where you extracted the **ASteCA** package.
4. Create a virtual environment with the command

   .. code-block:: bash

     $ conda create --name asteca python=3.9.12 pandas=1.4.2 matplotlib=3.5.1 numpy=1.22.3 scipy=1.7.3 astropy=5.0.4

5. Activate the environment

   .. code-block:: bash

    $ conda activate asteca

   (for Windows users the command is ``$ activate asteca``)

   .. important::

     You can tell that the environment is activated because its name is now
     shown in the terminal before the ``$`` symbol as:

     .. code-block:: bash

      (asteca) $

     You need to activate this environment each time *before* attempting to
     run **ASteCA**, otherwise no installed packages will be detected.

6. Finally, install the (optional) emcee and corner packages with:

   .. code-block:: bash

     $ conda install -c conda-forge emcee
     $ python -m pip install corner


.. _conda: https://conda.io/docs/index.html


Download
--------

The latest packaged release can be downloaded `from Github`_.
After downloading, extract the compressed file wherever you want
the code to exist. Alternatively the entire project can be cloned via `git`_
with (Linux command):

.. code-block:: bash

    $ git clone https://github.com/asteca/ASteCA.git

which will create a sub-folder named ``/ASteCA``.


First run
---------

With the environment activated and the code uncompressed into its folder,
you can run **ASteCA** with:

.. code-block:: bash

 (asteca) $ python asteca.py

This will produce a first run of the code that should finish successfully in
a few minutes.



.. _from Github: https://github.com/Gabriel-p/asteca/releases
.. _git: http://git-scm.com/