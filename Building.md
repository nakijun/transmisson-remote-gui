Make sure you have working [Lazarus](http://lazarus.freepascal.org) and [Free Pascal](http://www.freepascal.org) compiler installed.

**Free Pascal Compiler 2.6.2 and Lazarus 1.0 is used to develop Transmission Remote GUI. You may use different versions of FPC and Lazarus at your own risk.**

Download the sources archive and extract it to some folder or perform svn checkout.

**Building from the command line**

There are 2 methods:
  1. Using make (recommended):
    * Open terminal/command line prompt and cd to the sources folder;
    * Execute `make` command to build the application;
    * Execute `make zipdist` command to create a release .zip archive in the `Release` sub-folder.
  1. Using lazbuild:
    * Open terminal/command line prompt and cd to the sources folder;
    * Execute `lazbuild transgui.lpi` command to build the application.

**Building from Lazarus IDE**
  * Run Lazarus IDE;
  * You need to install the package with transgui custom components before opening the transgui project. The package installation is needed only once. To install the package do the following:
    * Select `"Package > Open package file (.lpk)..."` from the main menu.
    * Locate the `trcomp.lpk` file in the program's sources folder and open it.
    * Press the `Install` button in the package window.
    * You will be asked to rebuild Lazarus. Do it to finish the package installation.
  * Open `transgui.lpi` project and build it.