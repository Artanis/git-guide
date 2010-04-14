==========================
git Source Code Management
==========================
This guide will cover installing git on Windows systems with msysgit,
setting up a GitHub.com account for remote code hosting and
collaboration, and allowing git to connect to GitHub for pushing and
pulling changes.

Additionally, this guide will introduce you to git with a short
tutorial.

.. contents::

---------------------------
Installing git with msysgit
---------------------------
The first step is to install git on your system. On linux this is as
simple as using the package manager to download and install the
application for you, and on Mac computers you can install git with
MacPorts. On Windows you'll need a helper program like msysgit_.
msysgit creates a unix-like environment in which git can run. You can
either use the standard command-line git application through it, or
work through the graphic interface provided by msysgit.

At the time of writing the latest release of msysgit was
`Git-1.7.0.2-preview20100309`_, so download that and run it.

After the Welcome Screen, you'll be asked to read the GNU public
license, which msysgit is licensed under. You don't have to agree to it
to use the application, only if you are redistributing or altering the
application.

The next screen is a standard install location. It is recommended to
leave this on the default value (``Program Files/Git``) unless you have
another install location.

Next is an install options screen. You have the option of not placing
new icons on your desktop and in the quick launch menu on the taskbar,
which I leave to your preference. The second option group, Windows
Explorer Integration, offers to either add context menu entries (one
that opens a unix command line in the current folder, and another that
opens the graphical interface,) or to install git-cheetah (a
TortoiseSVN clone.) I recommend leaving the bottom two options alone.

The next screen asks where or if you'd like to install a Start Menu
entry. As this guide will assume you can access the application through
the Start Menu, please allow it to do so.

The next screen asks you about the PATH environment variable, which
tells the operating system where to find utility programs. I highly
recommend selecting the "Use Git Bash only" option, which makes no
changes to the PATH variable.

The final screen asks about line-ending characters. On Unix-like systems
the line-ending character is a single new-line character (``\n``), while
on Windows the line-ending characters are a carriage-return and
new-line (``\r\n``). This means that text files coming to windows from
a unix machine will appear all on one line, while files coming from
windows to a unix machine will have an extra trailing character on
each line. Choose "Checkout Windows-style, commit Unix-style line
endings," which will automatically convert files to windows line-ends
when you get them, and convert them to unix style when you commit them
to the repository.

The install of msysgit is complete. You can review the release notes or
just close out the installer.

.. _msysgit: http://code.google.com/p/msysgit/

.. _Git-1.7.0.2-preview20100309: http://msysgit.googlecode.com/files/Git-1.7.0.2-preview20100309.exe

------
GitHub
------
Once the local software is installed, the second step is to get the
code we are going to be working on, but we have some pre-requisites: the
service I am using to host the code is protecting the repository, so we
need to get in to that system first.

.. note::
    
    GitHub is an external service that hosts git repositories. You do
    not need a GitHub account to use git itself, or even public
    repositories hosted on GitHub, you only need a GitHub account to be
    able to access the private repositories hosted there.

For me the be able to add you to the repository, you will need a
`GitHub user account`_ (there are several pay options offered for larger
needs, choose the free option as we will not be needing the features
offered in those plans.)
