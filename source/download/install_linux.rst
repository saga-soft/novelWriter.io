.. _main_install_linux:

*******************
Installing on Linux
*******************

.. _GitHub: https://github.com/saga-soft/novelWriter
.. _PPA: https://launchpad.net/~vkbo/+archive/ubuntu/novelwriter
.. _Pre-Release PPA: https://launchpad.net/~vkbo/+archive/ubuntu/novelwriter-pre
.. _Releases: https://github.com/saga-soft/novelWriter/releases
.. _AppImage: https://appimage.org/
.. _Fedora repository: https://packages.fedoraproject.org/pkgs/novelwriter/novelwriter/
.. _Cloudsmith: https://cloudsmith.com/

There are different ways to install novelWriter, depending on your Linux distro. Here is a quick overview.


.. _main_install_linux_native:

Debian Linux Packages
=====================

Free package repository hosting is graciously provided by Cloudsmith_.

The Cloudsmith  repository contains native Linux packages for distros that have compatible system libraries for running
novelWriter. Currently supported are Debian 12 (Bookworm) and later, Ubuntu 24.04 (Noble) and later, Linux Mint 22
(Wilma) and later.

To add the package repositories to your local system, run the following command in a terminal:

.. code-block:: bash

   curl -sLf \
     'https://dl.cloudsmith.io/public/saga-soft/stable/cfg/setup/bash.deb.sh' \
     | sudo bash


If you also want to receive pre-release versions, run the following command:

.. code-block:: bash

   curl -sLf \
     'https://dl.cloudsmith.io/public/saga-soft/testing/cfg/setup/bash.deb.sh' \
     | sudo bash

You can have both set up at the same time.

**Other Debian-Based Distros**

If there is no dedicated package for your Debian-based distro, you can try installing the package for the closest
supported version by specifying those on the last line of the above commands:

.. code-block:: bash

   curl -sLf \
     'https://dl.cloudsmith.io/public/saga-soft/stable/cfg/setup/bash.deb.sh' \
     | sudo distro=DISTRO codename=VERSION bash


Installing novelWriter
----------------------

After the repository is set up, you can install novelWriter with the following command (Debian/Ubuntu/Mint):

.. code-block:: bash

   sudo apt update && sudo apt install novelwriter


.. _main_install_linux_fedora:

Fedora
======

novelWriter is available in the main `Fedora repository`_ as of Fedora 41.

You can install it with:

.. code-block:: bash

   sudo dnf install novelwriter


.. _main_install_linux_appimage:

AppImage Releases
=================

For other Linux distros than the ones mentioned above, the primary option is AppImage_. These are
completely standalone images for the app that include the necessary environment to run novelWriter.
They can of course be run on any Linux distro, if you prefer this to native packages.


Known Issues
------------

There are some known issues with the new AppImage files on some distros and desktop environments
after the switch to Qt6. If you get the following error:

.. code-block::

   qt.qpa.plugin: From 6.5.0, xcb-cursor0 or libxcb-cursor0 is needed to load the Qt xcb platform plugin.
   qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found.
   This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.

Try installing one of the suggested packages:

.. code-block:: bash

   sudo apt install libxcb-cursor0

A more permanent solution will come, but for the time being, installing the library should solve the issue.


.. _main_install_linux_chromeos:

ChromeOS
--------

On ChromeOS Linux (Crostini), some users have reported that the AppImage may fail to start with a
Wayland error. If this happens, run novelWriter with Qt forced to use the X11 backend.

.. code-block:: bash

   QT_QPA_PLATFORM=xcb /path/to/novelwriter.AppImage

For example:

.. code-block:: bash

   QT_QPA_PLATFORM=xcb ~/applications/novelwriter.AppImage

If you launch novelWriter from a desktop shortcut, you can make this permanent by adding
``QT_QPA_PLATFORM=xcb`` in front of the AppImage command in the launcher's ``Exec=`` line.
