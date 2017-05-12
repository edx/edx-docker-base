Part of `edX code`__.

__ http://code.edx.org/

edX Docker Images |Travis|_
===========================
.. |Travis| image:: https://travis-ci.org/edx/edx-docker-base.svg?branch=master
.. _Travis: https://travis-ci.org/edx/edx-docker-base


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

Mailing List and IRC Channel
----------------------------

You can discuss this code in the `edx-code Google Group`__ or in the ``#edx-code`` IRC channel on Freenode.

__ https://groups.google.com/forum/#!forum/edx-code
