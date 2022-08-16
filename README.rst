.. image:: https://img.shields.io/badge/tstn--036-lsst.io-brightgreen.svg
   :target: https://tstn-036.lsst.io
.. image:: https://github.com/lsst-tstn/tstn-036/workflows/CI/badge.svg
   :target: https://github.com/lsst-tstn/tstn-036/actions/
..
  Uncomment this section and modify the DOI strings to include a Zenodo DOI badge in the README
  .. image:: https://zenodo.org/badge/doi/10.5281/zenodo.#####.svg
     :target: http://dx.doi.org/10.5281/zenodo.#####

#####################################################
AuxTel Calibration Illumination Control with Lab Jack
#####################################################

TSTN-036
========

For the AuxTel Calibration Illumination system, we plan to use a LabJack T4 to control and communicate with the KiloArc White Light Source. We will use the same LabJack to control the Linear Actuator which opens the shutter for the beam. Below is a description of the I/O for the LabJack and corresponding rules for the operation of the elements described.

When the White Light Source (WLS) is being operated, a Chiller must also be running to cool the beam. The chiller will not be controlled using the LabJack but rather a Serial Device Server (Nport 5150A). Some of this had previously been implemented in a CSC for control by the ADAM-6024. The code can be found here: https://github.com/lsst-ts/ts_ATWhiteLightSource. Included below are some rules about operating the WLS with the Chiller. 

**Links:**

- Publication URL: https://tstn-036.lsst.io
- Alternative editions: https://tstn-036.lsst.io/v
- GitHub repository: https://github.com/lsst-tstn/tstn-036
- Build system: https://github.com/lsst-tstn/tstn-036/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally with `Sphinx`_:

.. code-block:: bash

   git clone https://github.com/lsst-tstn/tstn-036
   cd tstn-036
   pip install -r requirements.txt
   make html

.. note::

   In a Conda_ environment, ``pip install -r requirements.txt`` doesn't work as expected.
   Instead, ``pip`` install the packages listed in ``requirements.txt`` individually.

The built technote is located at ``_build/html/index.html``.

Editing this technical note
===========================

You can edit the ``index.rst`` file, which is a reStructuredText document.
The `DM reStructuredText Style Guide`_ is a good resource for how we write reStructuredText.

Remember that images and other types of assets should be stored in the ``_static/`` directory of this repository.
See ``_static/README.rst`` for more information.

The published technote at https://tstn-036.lsst.io will be automatically rebuilt whenever you push your changes to the ``main`` branch on `GitHub <https://github.com/lsst-tstn/tstn-036>`_.

Updating metadata
=================

This technote's metadata is maintained in ``metadata.yaml``.
In this metadata you can edit the technote's title, authors, publication date, etc..
``metadata.yaml`` is self-documenting with inline comments.

Using the bibliographies
========================

The bibliography files in ``lsstbib/`` are copies from `lsst-texmf`_.
You can update them to the current `lsst-texmf`_ versions with::

   make refresh-bib

Add new bibliography items to the ``local.bib`` file in the root directory (and later add them to `lsst-texmf`_).

.. _Sphinx: http://sphinx-doc.org
.. _DM reStructuredText Style Guide: https://developer.lsst.io/restructuredtext/style.html
.. _this repo: ./index.rst
.. _Conda: http://conda.pydata.org/docs/
.. _lsst-texmf: https://lsst-texmf.lsst.io
