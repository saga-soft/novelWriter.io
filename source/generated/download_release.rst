.. _AppImage: https://appimage.org/
.. _Flatpak: https://flatpak.org/
.. _Ubuntu: https://ubuntu.com/
.. _Debian: https://www.debian.org/
.. _Linux Mint: https://linuxmint.com/
.. _novelWriter Repository: https://github.com/saga-soft/novelWriter/
.. _SignPath.io: https://about.signpath.io/
.. _SignPath Foundation: https://signpath.org/
.. _PyPi: https://pypi.org/project/novelWriter/
.. _Cloudsmith: https://cloudsmith.com/

| **Release Version:** 2026.2
| **Release Date:** September 5, 2026
| **Release Notes:** :ref:`main_release_26_2`
| **Release Feedback:** :octicon:`comment-discussion` `Discussion <https://github.com/orgs/saga-soft/discussions/3005>`__
| **Release on GitHub:** :octicon:`mark-github` `GitHub <https://github.com/saga-soft/novelWriter/releases/tag/v26.2>`__

.. |linux-logo| image:: ../images/linux.svg
   :class: dark-light custom-inline-image-title

.. |windows10-logo| image:: ../images/windows10.svg
   :class: dark-light custom-inline-image-title

.. |package-logo| image:: ../images/package.png
   :class: dark-light custom-inline-image-title


Linux |linux-logo|
------------------

AppImage
^^^^^^^^

.. card::

   The AppImage_ should run on any recent Linux distro.

   :octicon:`download` `novelwriter-26.2-x86_64.AppImage <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-x86_64.AppImage>`__ [83.8 MB]
   :bdg-link-primary-line:`Checksum File <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-x86_64.AppImage.sha256>`


Flatpak (Experimental)
^^^^^^^^^^^^^^^^^^^^^^

.. card::

   The Flatpak_ should run on any recent Linux distro.

   :octicon:`download` `novelwriter-26.2-linux.flatpak <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-linux.flatpak>`__ [10.9 MB]
   :bdg-link-primary-line:`Checksum File <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-linux.flatpak.sha256>`


Debian Packages
^^^^^^^^^^^^^^^

.. card::

   Packages for Debian_, Ubuntu_ and `Linux Mint`_ can be downloaded from the Cloudsmith repository.

   | :octicon:`package` `Saga-Soft Repository (Stable) <https://broadcasts.cloudsmith.com/saga-soft/stable>`__

   See :ref:`main_install_linux` for more details.

   Free package repository hosting is graciously provided by Cloudsmith_.


Windows |windows10-logo|
------------------------

Setup Installer
^^^^^^^^^^^^^^^

.. card::

   This is a standard setup installer for Windows. It is made for Windows 10 or newer.

   :octicon:`download` `novelwriter-26.2-amd64-setup.exe <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-amd64-setup.exe>`__ [103 MB]
   :bdg-link-primary-line:`Checksum File <https://github.com/saga-soft/novelWriter/releases/download/v26.2/novelwriter-26.2-amd64-setup.exe.sha256>`

   Free code signing is provided by `SignPath.io`_, certificate by `SignPath Foundation`_.


Other Packages |package-logo|
-----------------------------

Python Wheel
^^^^^^^^^^^^

.. card::

   A standard Python wheel package is available for installation from PyPi_.

   .. code-block:: bash

      pipx install novelwriter==26.2

   See :ref:`main_install_pypi` for more details.


Source Code
^^^^^^^^^^^

.. card::

   The source code packages are archived files of the entire source code.

   | :octicon:`download` `novelWriter-26.2.zip <https://api.github.com/repos/saga-soft/novelWriter/zipball/v26.2>`__
   | :octicon:`download` `novelWriter-26.2.tar.gz <https://api.github.com/repos/saga-soft/novelWriter/tarball/v26.2>`__

   See also the `novelWriter Repository`_.

.. note::

   For the time being, the MacOS releases have been discontinued. There is currently no one available to maintain these
   releases. This is an open source project, and it depends on volunteers and contributors to run.
   See `this discussion <https://github.com/saga-soft/novelWriter/discussions/2618>`__ for more details.

   If you own a Mac and have a Python environment set up, you can still install the Python package of novelWriter and
   run the latest release. See :ref:`main_install_pypi` for more details.
