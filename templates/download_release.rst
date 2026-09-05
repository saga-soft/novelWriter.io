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

| **Release Version:** {release_version}
| **Release Date:** {release_date}
| **Release Notes:** :ref:`{release_ref}`
| **Release Feedback:** :octicon:`comment-discussion` `Discussion <{discuss_url}>`__
| **Release on GitHub:** :octicon:`mark-github` `GitHub <{release_url}>`__

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

   :octicon:`download` `{appimage_name} <{appimage_url}>`__ [{appimage_size}]
   :bdg-link-primary-line:`Checksum File <{appimage_shasumfile}>`


Flatpak (Experimental)
^^^^^^^^^^^^^^^^^^^^^^

.. card::

   The Flatpak_ should run on any recent Linux distro.

   :octicon:`download` `{flatpak_name} <{flatpak_url}>`__ [{flatpak_size}]
   :bdg-link-primary-line:`Checksum File <{flatpak_shasumfile}>`


Debian Packages
^^^^^^^^^^^^^^^

.. card::

   Packages for Debian_, Ubuntu_ and `Linux Mint`_ can be downloaded from the Cloudsmith repository.

   | :octicon:`package` `Saga-Soft Repository ({cloudsmith_repo}) <{cloudsmith_url}>`__

   See :ref:`main_install_linux` for more details.

   Free package repository hosting is graciously provided by Cloudsmith_.


Windows |windows10-logo|
------------------------

Setup Installer
^^^^^^^^^^^^^^^

.. card::

   This is a standard setup installer for Windows. It is made for Windows 10 or newer.

   :octicon:`download` `{winexe_name} <{winexe_url}>`__ [{winexe_size}]
   :bdg-link-primary-line:`Checksum File <{winexe_shasumfile}>`

   Free code signing is provided by `SignPath.io`_, certificate by `SignPath Foundation`_.


Other Packages |package-logo|
-----------------------------

Python Wheel
^^^^^^^^^^^^

.. card::

   A standard Python wheel package is available for installation from PyPi_.

   .. code-block:: bash

      pipx install novelwriter=={short_version}

   See :ref:`main_install_pypi` for more details.


Source Code
^^^^^^^^^^^

.. card::

   The source code packages are archived files of the entire source code.

   | :octicon:`download` `novelWriter-{short_version}.zip <{zip_url}>`__
   | :octicon:`download` `novelWriter-{short_version}.tar.gz <{tar_url}>`__

   See also the `novelWriter Repository`_.

.. note::

   For the time being, the MacOS releases have been discontinued. There is currently no one available to maintain these
   releases. This is an open source project, and it depends on volunteers and contributors to run.
   See `this discussion <https://github.com/saga-soft/novelWriter/discussions/2618>`__ for more details.

   If you own a Mac and have a Python environment set up, you can still install the Python package of novelWriter and
   run the latest release. See :ref:`main_install_pypi` for more details.
