Make reStructuredText by LeXtudio (RTL) working
===============================================

Below is a process of installing RTL in **Windows**.

0. Prerequisites: 
    * VS Code installed
    * Docs files from docs repo on Github were pulled to the working directory
    * You are familiar with recommended :ref:`official videos VS Code <official videos vs code>`

.. _rtl first step:

1. Check that Python is installed on your machine. :kbd:`⊞ Win` + :kbd:`cmd` and then print 

    .. code-block:: console

        py --version

    your version should be higher than ``3.8.0``. If you have no Python and never installed Python before, 
    check our :doc:`help here</start/contribute/python_install>`.
    If Python is missed or the version is old you 
    should get it from `official source`_. It is recommended to add ``python.exe`` to the path -- see
    checkbox on the initial screen before installation. In the end it is recommended to disable path limit.
    After installation is complete, reload VS Code to let the path to Python scripts updates.

2. In VS Code press :kbd:`⌃ Control` + :kbd:`⇧ Shift` + :kbd:`X` to open extension marketplace, find 
   `Python by Microsoft`_ and install.

    * In case of multiple Python installations choose the correct one by :kbd:`⌃ Control` + :kbd:`⇧ Shift` 
      + :kbd:`P` and command ``Python: Select Interpreter``

3. In VS Code press  :kbd:`⌃ Control` + :kbd:`⇧ Shift` + :kbd:`\`` to start terminal
   
    .. tip::
       :kbd:`\`` - ticks are typically below :kbd:`~` and to left from :kbd:`1` on the keyboard

    Then to install ``sphinx``,  blue-white_ RTD theme_, sphinx-copybutton_, other packages, mentioned in 
    ``./docs/requirements.txt``, and language server esbonio_ print the following command:

    .. code-block:: console

        pip install -r requirements.txt esbonio
    
.. caution:: 
   
   For correct work RTL requires some additional dependencies -- ``esbonio`` and ``reStructuredText Syntax highlighting``, 
   that will be prompted to you during installation of RTL, so be careful and agree to install them and later install esbonio server. 

4. In VS Code extension market find reStructuredText_ and press ``install``. Follow prompts to install dependencies 
   and run them. 

Congrat!
--------
Now you can use preview button |preview_ico| in VS Code on ``.rst`` files.


.. _official source: https://www.python.org/downloads/windows/
.. _Python by Microsoft: https://marketplace.visualstudio.com/items?itemName=ms-python.python
.. _blue-white: https://blog.readthedocs.com/new-theme-read-the-docs/
.. _theme: https://sphinx-rtd-theme.readthedocs.io/en/stable/
.. _sphinx-copybutton: https://sphinx-copybutton.readthedocs.io/en/latest/
.. _esBonio: https://github.com/swyddfa/esbonio
.. _reStructuredText: https://marketplace.visualstudio.com/items?itemName=lextudio.restructuredtext
.. |preview_ico| image:: /res/start/contribute/open-preview.svg

