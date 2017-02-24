{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
===============================
{{ cookiecutter.project_name }}
===============================

{% if is_open_source %}
.. image:: https://img.shields.io/travis/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}.svg
        :target: https://travis-ci.org/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}

.. image:: https://ci.appveyor.com/api/projects/status/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}?svg=true
        :target: https://ci.appveyor.com/api/projects/status/github/{{ cookiecutter.github_username }}/{{ cookiecutter.project_slug }}/branch/master

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

Quickstart
----------

These instructions assume you have just completed creating a repo with cookiecutter and have cd'ed into the repo


* Create the corresponding repo in Github.
* Add the repo to your Travis-CI_ account.
* Add the repo to your Appveyor_ account.
* Add the repo to your Coveralls_ account.
* `Git init`
* `Git add .`
* `Git commit -m "Initial commit"`
* follow the instructions from Github to point your local repo to Github and push your repo
* Update the badges
* Delete these instructions from this file.


Features
--------

* TODO

Credits
---------

This package was created with Cookiecutter_ and the `lneisenman/cookiecutter-python`_ project template which is based on the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`lneisenman/cookiecutter-python`: https://github.com/lneisenman/cookiecutter-python
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
.. _Appveyor: https://ci.appveyor.com/
.. _Coveralls: https://coveralls.io/
.. _Travis-CI: http://travis-ci.org/
