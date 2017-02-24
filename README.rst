======================
Cookiecutter Python
======================



Cookiecutter_ template for a Python package based on audreyr's cookiecutter-pypackage_.

* GitHub repo: https://github.com/lneisenman/cookiecutter-python/
* Documentation: https://cookiecutter-pypackage.readthedocs.io/
* Free software: BSD license

.. _`cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage

Features
--------

* Testing setup with ``pytest``
* Travis-CI_: Ready for Travis Continuous Integration testing
* Appveyor: Ready for Appveyor Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 2.7, 3.5, 3.6
* Sphinx_ docs: Documentation ready for generation with, for example, ReadTheDocs_
* Bumpversion_: Pre-configured version bumping with a single command
* Auto-release to PyPI_ when you push a new tag to master (optional)
* Command line interface using Click (optional)


Build Status
-------------

Linux:

.. image:: https://img.shields.io/travis/lneisenman/cookiecutter-python.svg
    :target: https://travis-ci.org/audreyr/cookiecutter-python
    :alt: Linux build status on Travis CI

Windows:

.. image:: https://ci.appveyor.com/api/projects/status/github/lneisenman/cookiecutter-python?branch=master
    :target: https://ci.appveyor.com/project/lneisenman/cookiecutter-python/branch/master
    :alt: Windows build status on Appveyor

Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter gh:lneisenman/cookiecutter-python

Then:

* Create the corresponding repo in Github.
* Add the repo to your Travis-CI_ account.
* Add the repo to your Appveyor account.
* Add the repo to your Coveralls account.
* `Git init`
* `Git add .`
* `Git commit -m "Initial commit"`
* follow the instructions from Github to point your local repo to Github and push your repo
* Update the badges
* Run the script `travis_pypi_setup.py` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch. (Optional)
* Add the repo to your ReadTheDocs_ account + turn on the ReadTheDocs service hook.
* Release your package by pushing a new tag to master.


For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html


