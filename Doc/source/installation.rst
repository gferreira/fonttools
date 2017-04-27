Installation
============

FontTools requires `Python <http://www.python.org/download/>`__ 2.7, 3.4 or later.

The package is listed in the Python Package Index (PyPI), so you can install it with `pip <https://pip.pypa.io>`__:

.. code:: sh

    pip install fonttools

If you would like to contribute to its development, you can clone the repository from Github, install the package in 'editable' mode and modify the source code in place. We recommend creating a virtual environment, using `virtualenv <https://virtualenv.pypa.io>`__ or Python 3 `venv <https://docs.python.org/3/library/venv.html>`__ module.

.. code:: sh

    # download the source code to 'fonttools' folder
    git clone https://github.com/fonttools/fonttools.git
    cd fonttools

    # create new virtual environment called e.g. 'fonttools-venv', or anything you like
    python -m virtualenv fonttools-venv

    # source the `activate` shell script to enter the environment (Un\*x); to exit, just type `deactivate`
    . fonttools-venv/bin/activate

    # to activate the virtual environment in Windows `cmd.exe`, do
    fonttools-venv\Scripts\activate.bat

    # install in 'editable' mode
    pip install -e .
