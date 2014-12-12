hg-scripts
==========

These scripts recursively check the status of all Mercurial repositories in a
given directory.

* *uncommitted* checks the repositories for uncommitted changes.
* *unpulled* checks the repositories for unpulled changes.
* *unpushed* checks the repositories for unpushed changes.

Usage
-----

.. sourcecode:: sh

    $ uncommitted ~/myrepos
    /home/user/myrepos/myapp/
    ? README.rst
