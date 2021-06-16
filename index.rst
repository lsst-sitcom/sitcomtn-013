..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. note::

    This technical note describes the deliverables of the First-look Analysis and Feedback Functionality Breakout Group.
    This is the initial draft and is not yet finalized

Context
========
The project is currently developing numerous tools to perform analysis of system performance, data acquisition, and display.
However, the majority of these tools have been designed to work for isolated use-cases that generally encompass the requirements of a single subsystem.
Commissioning and operating the observatory will require a more cross-subsystem approach, specifically when dealing with on-the-fly analysis and display of data on the mountain, which may originate from any of the subsystems but needs to be displayed and/or communicated to the operator in a coherent and timely fashion.

Motivation
==========
To date, there exists no concrete strategy nor workflow on how the project will perform on-the-fly data analyses and display this information to the operator.
Commissioning has now started with regular auxTel observing, and these tools would already be in use if they existed.
These tools and workflows need to be in regular use and well developed before moving into the on-sky commissioning period with ComCam.

Scope and Deliverables
======================
This group is being assembled to review the current strategies and tooling of the project, and evaluate the approach against a series of typical use-cases that demonstrate critical functionalities to observatory commissioning and operations.
The group will report the finding and make a series of recommendations to augment the current tools and possibly design and develop new tools to address the use-cases.

The following items shall be delivered by the group:

#. A series of use-cases where feedback to observers is required. A reduced set of use-cases should be created as a regular reference during design and development.

    - Use-cases should be complete, including which inputs are required (e.g. SAL Script, EFD, LFA, external source), desired manipulations, logic-based operations/calculations, and how the desired artefacts are presented to the user (e.g. display images and/or graphs).

#. A set of requirements to augment, clarify, or remove ambiguity that may occur from looking only at the use-cases.

    - This is not a formal and all-encompassing LSE requirements document.

#. A summary of the suite of currently available tools/systems that may help fulfil the required functionality.

    - Report on their status, limitations, and where their current requirements may need to be expanded to cover any increase in scope
    - Tools which were considered but found to be inadequate must also be reported

#. A mapping of the use-cases into the currently available systems, clearly identifying where new functionality is required.

    - This could be by augmenting current systems or the creation of a new system if required
    - Deliver a proposed implementation for each use-case

#. A prioritized list of tasks to build-out the new functionalities with recommended end-dates. These dates shall correspond to integration milestones.


Timeline
========
This group is to complete items 1-4 of this charge by August 2nd, with item 5 to be completed by August 14th.

Aspects Considered Out-Of-Scope
===============================

#. Creation of the LCR to support the effort

    - This is to be completed by a SIT-Com manager

#. Scheduling of the tasks by the subsystems
#. Design of the components and/or systems to incorporate any new functionality

Participants
============

- Patrick Ingraham (chair): Calibration Systems Engineer

- Keith Bechtol: Commissioning Scientist and Associate Professor at the University of Wisconsin

- Tony Johnson: Camera Control Software Lead

- Simon Krughoff: SQuaRE Science Lead

- Kian-Tat Lim: DM Software Architect

- Robert Lupton: Calibration Scientist

- Tiago Ribeiro: T&S Software Architect and Scheduler Scientist


.. Add content here.
.. Do not include the document title (it's automatically added from metadata.yaml).

.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
