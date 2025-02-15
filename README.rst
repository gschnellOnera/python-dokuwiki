python-dokuwiki
===============

.. image:: https://img.shields.io/badge/github-repo-yellow.jpg
           :target: https://github.com/fmenabe/python-dokuwiki
           :alt: Code repo

.. image:: https://img.shields.io/pypi/v/dokuwiki.svg
           :target: https://pypi.python.org/pypi/dokuwiki
           :alt: PyPi

.. image:: https://readthedocs.org/projects/python-dokuwiki/badge/?version=latest
           :target: http://python-dokuwiki.readthedocs.org/en/latest/
           :alt: Documentation

.. image:: https://landscape.io/github/fmenabe/python-dokuwiki/master/landscape.svg?style=flat
           :target: https://landscape.io/github/fmenabe/python-dokuwiki/master
           :alt: Code Health

.. .. image:: https://img.shields.io/pypi/dm/dokuwiki.svg
              :target: https://pypi.python.org/pypi/dokuwiki
              :alt: Downloads


This python module aims to manage `DokuWiki <https://www.dokuwiki.org/dokuwiki>`_
wikis by using the provided `XML-RPC API <https://www.dokuwiki.org/devel:xmlrpc>`_.
This module is compatible with python2.7 and python3+.

API is described `here <http://python-dokuwiki.readthedocs.org/en/latest/>`_.


Release notes
-------------

1.3.2 (2021-12-03)
~~~~~~~~~~~~~~~~~~
    * Correct a bug when using some special characters in the password (`c891eb8
      <https://github.com/fmenabe/python-dokuwiki/commit/c891eb8>`_)

1.3.1 (2021-08-30)
~~~~~~~~~~~~~~~~~~
    * Set default empty value for `summary` to `structs.get_data()`
    * Add `minor` parameter to `structs.get_data()`

1.2.1 (2019-07-24)
~~~~~~~~~~~~~~~~~~
    * Remove `login <https://www.dokuwiki.org/devel:xmlrpc#dokuwikilogin>`_ call
      in the constructor as it seems to fail on some cases (`98ed799
      <https://github.com/fmenabe/python-dokuwiki/commit/98ed799>`_).

1.2.0 (2019-06-25)
~~~~~~~~~~~~~~~~~~
    * Support of HTTPS for cookie based authentication.

1.1.0 (2018-03-22)
~~~~~~~~~~~~~~~~~~
    * Support authentication by cookie (thanks to *luminisward*).

1.0.1 (2017-04-06)
~~~~~~~~~~~~~~~~~~
    * Correct a typo with an exception call.

1.0 (2017-04-06)
~~~~~~~~~~~~~~~~
    * Prevent username and password to be passed as GET parameters (`e4cbb5d <https://github.com/fmenabe/python-dokuwiki/commit/e4cbb5d>`_).

0.5 (2016-08-19)
~~~~~~~~~~~~~~~~
    * Correct a bug when retrieving/uploading medias (`a1f56b6 <https://github.com/fmenabe/python-dokuwiki/commit/a1f56b6>`_).

0.4 (2016-02-07)
~~~~~~~~~~~~~~~~
    * Allow media to be get/set as bytes (`44c6dcf <https://github.com/fmenabe/python-dokuwiki/commit/44c6dcf>`_, `1621291 <https://github.com/fmenabe/python-dokuwiki/commit/1621291>`_)
    * Force login after XML-RPC initialization for ensuring the connection is working (`55ffff8 <https://github.com/fmenabe/python-dokuwiki/commit/55ffff8>`_)
    * Fix minor bugs (`d5b7163 <https://github.com/fmenabe/python-dokuwiki/commit/d5b7163>`_, `9b164ea <https://github.com/fmenabe/python-dokuwiki/commit/9b164ea>`_)
    * Add sphinx documentation based on docstrings (`74968dc <https://github.com/fmenabe/python-dokuwiki/commit/74968dc>`_, `c8e1503 <https://github.com/fmenabe/python-dokuwiki/commit/c8e1503>`_)

0.3 (2015-08-16)
~~~~~~~~~~~~~~~~
    * The xmlrpc parameter ``use_datetime`` is no longer forced to *True* by default (`bec3447 <https://github.com/fmenabe/python-dokuwiki/commit/bec3447>`_). **This may break things!**

0.2 (2014-01-29)
~~~~~~~~~~~~~~~~
    * Manage dataentries (this is a plugin for managing metadatas).

0.1 (2014-01-29)
~~~~~~~~~~~~~~~~
    * Implement DokuWiki XML-RPC commands.
    * Compatible with both python 2 and 3.
