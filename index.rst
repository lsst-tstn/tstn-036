:tocdepth: 1

.. sectnum::

.. Metadata such as the title, authors, and description are set in metadata.yaml

.. TODO: Delete the note below before merging new content to the main branch.

.. note::

   **This technote is a work-in-progress.**

Abstract
========

For the AuxTel Calibration Illumination system, we plan to use a LabJack T4 to control and communicate with the KiloArc White Light Source. We will use the same LabJack to control the Linear Actuator which opens the shutter for the beam. Below is a description of the I/O for the LabJack and corresponding rules for the operation of the elements described.

When the White Light Source (WLS) is being operated, a Chiller must also be running to cool the beam. The chiller will not be controlled using the LabJack but rather a Serial Device Server (Nport 5150A). Some of this had previously been implemented in a CSC for control by the ADAM-6024. The code can be found here: https://github.com/lsst-ts/ts_ATWhiteLightSource. Included below are some rules about operating the WLS with the Chiller. 

Add content here
================

Add content here.
See the `reStructuredText Style Guide <https://developer.lsst.io/restructuredtext/style.html>`__ to learn how to create sections, links, images, tables, equations, and more.

.. Make in-text citations with: :cite:`bibkey`.
.. Uncomment to use citations
.. .. rubric:: References
.. 
.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
