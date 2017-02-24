{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
===============================
{{ cookiecutter.project_name }}
===============================

{% if is_open_source %}
.. image:: https://img.shields.io/travis/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}.svg
        :target: https://travis-ci.org/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}

.. image:: https://ci.appveyor.com/api/projects/status/liiq6hget4c6etug?svg=true
        :target: https://ci.appveyor.com/api/projects/status/liiq6hget4c6etug

.. image:: https://coveralls.io/repos/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/badge.svg?branch=master
        :target: https://coveralls.io/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}?branch=master

.. image:: https://readthedocs.org/projects/{{ cookiecutter.project_slug | replace("_", "-") }}/badge/?version=latest
        :target: https://{{ cookiecutter.project_slug | replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status
{%- endif %}


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

This package was created with Cookiecutter_ and the `lneisenman/cookiecutter-python`_ project template which is based on the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`lneisenman/cookiecutter-python`: https://github.com/lneisenman/cookiecutter-python
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
