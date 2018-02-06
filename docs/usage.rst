=====
Usage
=====

To use quartet_manifest in a project, add it to your `INSTALLED_APPS`:

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
