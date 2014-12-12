hg-scripts
==========

Recursively check the status of all Mercurial repositories in a given directory.

* *uncommitted* checks the repositories for uncommitted changes.
* *unpulled* checks the repositories for unpulled changes.
* *unpushed* checks the repositories for unpushed changes.

Usage
-----

.. sourcecode:: sh

    $ uncommitted ~/myrepos
    /home/user/myrepos/myapp/
    ? README.rst
    $ hg ci -R ~/myrepos/myapp -m 'Added readme'
    $ unpulled ~/myrepos
    $ unpushed ~/myrepos
    /home/user/myrepos/myapp/
    summary:    Updated readme
    $ hg push -R ~/myrepos/myapp
    pushing to ...
