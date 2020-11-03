![LibreOffice](LibreOffice.png)

---

LibreOffice is a free and powerful office suite, and a successor to OpenOffice.org (commonly known as OpenOffice).  Its clean interface and feature-rich tools help you unleash your creativity and enhance your productivity.

How to build LibreOffice
------------------------

-   Read our documentation on [how to build LibreOffice](https://wiki.documentfoundation.org/Development/How_to_build)
-   Read our overview of [the build system](https://wiki.documentfoundation.org/Development/Build_System)
-   Watch a quick video intro on [how to build LibreOffice](https://www.youtube.com/watch?v=2gIqOOajdYQ&hd=1)
-   Watch a video tutorial on [hacking LibreOffice with Kdevelop](https://www.youtube.com/watch?v=-5hVXeHNt2M) 

There are three ways to get the source code:

-   Clone from [Gerrit](https://gerrit.libreoffice.org/) (our code review tool):** git clone https://git.libreoffice.org/core\
    **
-   Clone from [the anongit repository](https://cgit.freedesktop.org/libreoffice): **git clone https://anongit.freedesktop.org/git/libreoffice/core.git**
-   As a final fallback, download [the tarball](https://dev-www.libreoffice.org/bundles/libreoffice-core.tar.bz2) (in case the Git server is experiencing problems). After downloading the tarball, follow these steps in your command line (for Windows it is assumed you are using cygwin shell):

> 1.  unpack the archive by running **tar xvf libreoffice-core.tar.bz2**
> 2.  change directory to "libo"
> 3.  run **git checkout -f**
> 4.  run **git pull -r** to get most recent commits

-   [Release tarballs](http://download.documentfoundation.org/libreoffice/src/) are only for people building LibreOffice for *nix distributions. Please find the latest versions (usually near the bottom)

Build and run it
----------------

These instructions are primarily aimed at a GNU/Linux user. Bootstrap your system by installing all the packages required to build your distribution's LibreOffice package. Refer to [the article on Linux build dependencies](https://wiki.documentfoundation.org/Development/Linux_Build_Dependencies) to make sure you get everything you need.

Then download the complete source code and build it:

**./autogen.sh**\
**make**

Start the program by running:** instdir/program/soffice**

Or use this command to start LibreOffice under the gdb debugger:

**make debugrun**

If you have problems with the build, don't be put off - get in touch with us on [IRC](https://irc.documentfoundation.org/?settings=#libreoffice-dev), and/or read the wiki page [How to build](https://wiki.documentfoundation.org/Development/How_to_build).
