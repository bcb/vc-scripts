hg-scripts
==========

Recursively check the status of all Mercurial repositories in a given directory.

* *uncommitted* shows uncommitted changes.
* *unpulled* shows unpulled changes.
* *unpushed* shows unpushed changes.

Usage
-----

.. sourcecode:: sh

    $ uncommitted ~/myrepos
    /home/user/myrepos/myapp/
    M README.rst
    $ hg ci -R ~/myrepos/myapp -m 'Updated readme'
    $ unpulled ~/myrepos
    $ unpushed ~/myrepos
    /home/user/myrepos/myapp/
    summary:    Updated readme
    $ hg push -R ~/myrepos/myapp
    pushing to ...
