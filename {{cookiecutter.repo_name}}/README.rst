{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
===============================
{{ cookiecutter.project_name }}
===============================

{% if is_open_source %}
.. image:: https://badge.fury.io/py/{{ cookiecutter.repo_name }}.svg
        :target: https://pypi.python.org/pypi/{{ cookiecutter.repo_name }}

.. image:: https://img.shields.io/travis/{{ cookiecutter.github_username }}/{{ cookiecutter.repo_name }}.svg
        :target: https://travis-ci.org/{{ cookiecutter.github_username }}/{{ cookiecutter.repo_name }}

.. image:: https://readthedocs.org/projects/{{ cookiecutter.repo_name | replace("_", "-") }}/badge/?version=latest
        :target: https://{{ cookiecutter.repo_name | replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status
{%- endif %}

.. image:: https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.repo_name }}/shield.svg
     :target: https://pyup.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.repo_name }}/
     :alt: Updates


{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Free software: {{ cookiecutter.open_source_license }}
* Documentation: https://{{ cookiecutter.project_slug | replace("_", "-") }}.readthedocs.io.
{% endif %}

Features
--------

* TODO

Credits
---------
Tools used in rendering this package:

* Cookiecutter_
* `cookiecutter-pypackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-pypackage`: https://github.com/condereis/cookiecutter-pypackage

