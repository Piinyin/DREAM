Welcome to DREAM documentation!
===============================

.. image:: imgs/logo.png
    :align: center
    :scale: 35 %
    :alt: DREAM!

Deep Report for AI Models (DREAM for short) is a Python package for model training, testing and building model card reports. 

Highlights
==========

- **Intuitive, fast deployment and reproducible**: interactive UI for feature selection and customization
- **Comprehensive documentation**: each method has a detailed explanation
- **Unit tested**: we provide unit tests for each feature
- **Easily extended**: adding new features is easy and we encourage you to contribute with your custom features

Contents
========

.. toctree::
   :maxdepth: 2

   Get Started <descriptions/get_started>
   Feature List <descriptions/feature_list>
   Personalised Features <descriptions/personal>
   Frequently Asked Questions <descriptions/faq>
   Module Reference <descriptions/modules>
   Authors <authors>
   Changelog <changelog>
   License <license>

Installation
============

Installation can be easily done with ``pip``:

.. code:: bash

    $ pip install dream

Get started
===========

The code below extracts all the available features on an example dataset.

.. code:: python

    import dream
    import pandas as pd

    # load dataset
    df = pd.read_csv('Dataset.txt')

    # Retrieves a pre-defined feature configuration file to extract all available features
    cfg = dream.get_features_by_domain()

    # Extract features
    X = dream.time_series_features_extractor(cfg, df)

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
