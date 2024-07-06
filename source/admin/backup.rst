Backup
++++++

Backup db for Docker Installation
---------------------------------

If you run Kuwaiba in Docker there are two options

1. *recommended* :  ``/data`` is in volume
2. ``/data`` was not in volume
3. ``/data`` is mounted and available from disk
   
Case #3 is trivial, you may simply backup the directory.

Case #1 is more complicated.

Case #1
~~~~~~~

Case #2
~~~~~~~

to copy files from container run

.. code-block:: console
     
    docker cp <container>:/data /path/to/backup

