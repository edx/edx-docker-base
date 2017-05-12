Part of `edX code`__.

__ http://code.edx.org/

edX Docker Images
=================

|travis-badge| |license-badge|


This repository contains base Docker image definitions for edX.

Images
------

======  =======================================================================
Image   Description
======  =======================================================================
Python  The Python images are based on the `official slim Python images`_. They
        are intended for use with our IDAs (micro-services), thus come with
        certain libraries pre-installed (e.g. ``gettext``, ``libssl``,
        ``libjpeg``).
======  =======================================================================

.. _official slim Python images: https://hub.docker.com/_/python/

Automated Builds
----------------

Images are built for every pull request and commit to the master branch. The images are pushed to Docker Hub after each
successful build of the master branch.

License
-------

The code in this repository is licensed under LICENSE_TYPE unless
otherwise noted.

Please see ``LICENSE`` for details.

How To Contribute
-----------------

Contributions are very welcome.

Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.

Even though they were written with ``edx-platform`` in mind, the guidelines
should be followed for Open edX code in general.

Reporting Security Issues
-------------------------

Please do not report security issues in public. Please email security@edx.org.

Getting Help
------------

Have a question about this repository, or about Open edX in general?  Please
refer to this `list of resources`_ if you need any assistance.

.. _list of resources: https://open.edx.org/getting-help

.. |travis-badge| image:: https://travis-ci.org/edx/edx-docker-base.svg?branch=master
    :target: https://travis-ci.org/edx/edx-docker-base
    :alt: Travis

.. |license-badge| image:: https://img.shields.io/github/license/edx/edx-docker-base.svg
    :target: https://github.com/edx/edx-docker-base/blob/master/LICENSE
    :alt: License
