Testing
=======

To run the test suite, you can do:

.. code:: sh

    python setup.py test

If you have `pytest <http://docs.pytest.org/en/latest/>`__, you can run
the ``pytest`` command directly. The tests will run against the
installed ``fontTools`` package, or the first one found in the
``PYTHONPATH``.

You can also use `tox <https://testrun.org/tox/latest/>`__ to
automatically run tests on different Python versions in isolated virtual
environments.

.. code:: sh

    pip install tox
    tox

Note that when you run ``tox`` without arguments, the tests are executed
for all the environments listed in tox.ini's ``envlist``. In our case,
this includes Python 2.7 and 3.6, so for this to work the ``python2.7``
and ``python3.6`` executables must be available in your ``PATH``.

You can specify an alternative environment list via the ``-e`` option,
or the ``TOXENV`` environment variable:

.. code:: sh

    tox -e py27-nocov
    TOXENV="py36-cov,htmlcov" tox
