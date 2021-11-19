djangorestframework-rapidjson
=============================

Provides `rapidjson <https://github.com/python-rapidjson/python-rapidjson>`_
support with parser and renderer.

.. image:: https://github.com/Onemind-Services-LLC/django-rest-framework-rapidjson/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/Onemind-Services-LLC/django-rest-framework-rapidjson/actions/workflows/ci.yml


How to install
--------------

.. code:: shell

    pip install git+https://github.com/Onemind-Services-LLC/django-rest-framework-rapidjson.git


How to use
----------

Update django rest framework config

.. code:: python

    REST_FRAMEWORK = {
        'DEFAULT_RENDERER_CLASSES': (
            'rest_framework_rapidjson.renderers.RapidJSONRenderer',
        ),
        'DEFAULT_PARSER_CLASSES': (
            'rest_framework_rapidjson.parsers.RapidJSONParser',
        )
    }
