vc-scripts
==========

Recursively check the status of version control repositories.

uncommitted
    Shows uncommitted changes.
unpulled
    Shows unpulled changes.
unpushed
    Shows unpushed changes.

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
