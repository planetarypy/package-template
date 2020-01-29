============================
PlanetaryPy package template
============================

..  image:: https://pyup.io/repos/github/audreyr/cookiecutter-pypackage/shield.svg
..      :target: https://pyup.io/repos/github/audreyr/cookiecutter-pypackage/
..     :alt: Updates

..  image:: https://travis-ci.org/audreyr/cookiecutter-pypackage.svg?branch=master
..    :target: https://travis-ci.org/audreyr/cookiecutter-pypackage

This is a package template provided by the PlanetaryPy project.

Using this template, packages can make use of the setup, installation,
and documentation infrastructure developed for the ``planetarypy``
core and affiliated packages.

* GitHub repo: https://github.com/planetarypy/package-template/
.. * Documentation: https://cookiecutter-pypackage.readthedocs.io/
* Free software: BSD license

Features
--------

* Testing setup with ``unittest`` and ``python setup.py test`` or ``pytest``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 3.5, 3.6, 3.7, 3.8
* Sphinx_ docs: Documentation ready for generation with, for example, ReadTheDocs_
* bump2version_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click (optional)

.. _Cookiecutter: https://github.com/audreyr/cookiecutter


Quickstart
----------

This package template makes use of the `cookiecutter`_ package to
make it easier to get started with the package template. You will
need to install cookiecutter which can be done easily using conda
or pip.

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher) via conda::

    conda install -c conda-forge cookiecutter

... or via pip::

    pip install -U cookiecutter


Generate a Python package project::

    cookiecutter gh:planetarypy/package-template

This will ask you a series of questions to configure your package, unless you
downloaded the cookiecutter.json file in this repo, and modified it for your use,
in which case you can::

    cookiecutter --config-file my_project.json gh:planetarypy/package-template

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``)
* Register_ your project with PyPI.
* Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your ReadTheDocs_ account + turn on the ReadTheDocs service hook.
* Release your package by pushing a new tag to master.
* Add a `requirements.txt` file that specifies the packages you will need for
  your project and their versions. For more info see the `pip docs for requirements files`_.
* Activate your project on `pyup.io`_.

.. _`pip docs for requirements files`: https://pip.pypa.io/en/stable/user_guide/#requirements-files
.. _Register: https://packaging.python.org/tutorials/packaging-projects/#uploading-the-distribution-archives

For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html


.. _Travis-CI: http://travis-ci.org/
.. _Tox: http://testrun.org/tox/
.. _Sphinx: http://sphinx-doc.org/
.. _ReadTheDocs: https://readthedocs.io/
.. _`pyup.io`: https://pyup.io/
.. _bump2version: https://github.com/c4urself/bump2version
.. _Punch: https://github.com/lgiordani/punch
.. _Pipenv: https://pipenv.readthedocs.io/en/latest/
.. _PyPi: https://pypi.python.org/pypi
