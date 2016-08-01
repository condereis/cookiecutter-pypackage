======================
Cookiecutter PyPackage
======================

This is a fork of `audreyr's cookiecutter-pypackage`_, with an additional attribute called repo_name. This way it is possible to have two different names for the outer repo folder and the inner project folder. The repo_name will be the one you use on pip (pip install <repo_name>) and the project_slug will be used when importing the package (import <project_slug>).

.. _`audreyr's cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage

For information on the original project:

* GitHub repo: https://github.com/audreyr/cookiecutter-pypackage/
* Documentation: https://cookiecutter-pypackage.readthedocs.io/



Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/condereis/cookiecutter-pypackage.git

Then:

* Create a repo and put it there.
* Add the repo to your Travis-CI_ account.
* Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``)
* Run the script `travis_pypi_setup.py` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
* Add the repo to your ReadTheDocs_ account + turn on the ReadTheDocs service hook.
* Release your package by pushing a new tag to master.
* Add a `requirements.txt` file that specifies the packages you will need for
  your project and their versions. For more info see the `pip docs for requirements files`_.
* Activate your project on `pyup.io`_.

.. _`pip docs for requirements files`: https://pip.pypa.io/en/stable/user_guide/#requirements-files

For more details, see the `cookiecutter-pypackage tutorial`_.

.. _`cookiecutter-pypackage tutorial`: https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html


