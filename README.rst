=============================
quartet_manifest
=============================

.. image:: https://badge.fury.io/py/quartet_manifest.svg
    :target: https://badge.fury.io/py/quartet_manifest

.. image:: https://travis-ci.org/serial-lab/quartet_manifest.svg?branch=master
    :target: https://travis-ci.org/serial-lab/quartet_manifest

.. image:: https://codecov.io/gh/serial-lab/quartet_manifest/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/serial-lab/quartet_manifest

Reports back configuration and capabilities to quartet-ui.

Documentation
-------------

The full documentation is at https://quartet_manifest.readthedocs.io.

Quickstart
----------

Install quartet_manifest::

    pip install quartet_manifest

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'quartet_manifest.apps.QuartetManifestConfig',
        ...
    )

Add quartet_manifest's URL patterns:

.. code-block:: python

    from quartet_manifest import urls as quartet_manifest_urls


    urlpatterns = [
        ...
        url(r'^', include(quartet_manifest_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
