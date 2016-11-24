============
Writing docs
============

Docs here are written using the ReStructuredText language (similar to markdown)
and rended using sphinx.

Some useful links to get started with each of these:

- http://docutils.sourceforge.net/docs/user/rst/quickstart.html
- http://docutils.sourceforge.net/docs/user/rst/quickref.html
- http://www.sphinx-doc.org/en/1.4.9/contents.html

Editing docs
============

These docs live here: https://github.com/abersailbot/documentation

To edit, do what you'd do with any other git repo: clone the repo and make your
changes. When possible, prefer creating a pull request to allow another set of
eyes to look it over.

Creating new pages
==================

1. Create a new rst file: e.g. ``doot.rst``
2. Add a title to the page
3. link to this file in ``index.rst`` along with the other pages:

   .. code-block:: rst
      
       .. toctree::
          :maxdepth: 2

          wiring-standard
          hardware-spec
          provisioning
          testing
          doot
