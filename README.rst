erunit
======

A root-less wrapper around runit

Keep in mind that this is work in progress code, with hardly any error handling.

Quick start
===========

Example with a first deployment, once ``erunit`` is in ``$PATH``.

::

    erunit init
    erunit runsvdir-start
    erunit new syncthing 'syncthing -no-browser'
    erunit enable syncthing

After that one may want to add ``@reboot erunit runsvdir-start`` to crontab to autostart erunit's runsvdir on system start.
