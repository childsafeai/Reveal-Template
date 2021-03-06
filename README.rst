***************
childsafe.ai Reveal Template
***************

A template project for `Reveal.js`_ presentations used for my `childsafe.ai`_ talks.


**Table of Contents**


.. contents::
    :local:
    :depth: 1
    :backlinks: none


Features
============

* Photo cards
* Headline cards
* Charts with `C3`_
* Map cards with `Google Maps`_
* Funnel and Pyramid charts with `Highcharts`_
* Network visualizations with `Viz.js`_
* YouTube embeds


Installation
============

Clone repo

.. code-block:: bash

    $ git clone https://github.com/childsafeai/Reveal-Template.git 


Install ``gulp`` and ``bower``

.. code-block:: bash
    
    $ npm install -g bower gulp

Install node dependencies

.. code-block:: bash

    $ npm install

Install client dependencies

.. code-block:: bash

    $ bower install

Serve presentation 

.. code-block:: bash
    
    $ gulp serve


Deploy to Heroku
================

This template comes with some helpers to make it easy to deploy your
presentations to Heroku.  Once you have cloned the repo and built your
presentation, use the following steps to deploy the presentation to Heroku.

Create Heroku app.

.. code-block:: bash

    $ heroku create

Configure Heroku app to use both Node and Python buildpacks. 
.. code-block:: bash

    $ heroku buildpacks:set heroku/nodejs
    $ heroku buildpacks:add --index 1 heroku/python

Push your presentation to Heroku

.. code-block:: bash

    $ git push heroku master

Open the presentation on your newly deployed host.

.. code-block:: bash

    $ heroku open


Meta
===========

* Written by `Rob Spectre`_
* Released under `MIT License`_
* Software is as is - no warranty expressed or implied.

.. _childsafe.ai: https://childsafe.ai
.. _Reveal.js: http://lab.hakim.se/reveal-js/
.. _C3: http://c3js.org/
.. _Google Maps: https://developers.google.com/maps/documentation/javascript/
.. _Highcharts: http://www.highcharts.com/
.. _Viz.js: http://visjs.org/
.. _Rob Spectre: http://www.brooklynhacker.com
.. _MIT License: http://opensource.org/licenses/MIT
