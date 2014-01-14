WeaponX Source
===================
To get started with WeaponX, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/version-control.html).

Create the Directories
----------------------

You will need to set up some directories in your build environment.

To create them run:

    mkdir -p ~/bin
    mkdir -p ~/weaponx

Install the Repository
----------------------

Enter the following to download the "repo" binary:

    curl https://dl-ssl.google.com/dl/googlesource/git-repo/repo > ~/bin/repo

    chmod a+x ~/bin/repo

You may need to reboot for these changes to take effect. 
Now enter the following to initialize the repository:

    cd ~/weapon

Repositories:
---------------

Before you continue --> run this in the terminal

    repo init -u git://github.com/WeaponX1/android.git -b wx44

    repo sync

Building the System
---------------

Initialize the environment with the envsetup.sh script. Note that replacing "source" with a single dot saves a few characters, and the short form is more commonly used in documentation.

    . build/envsetup.sh

    lunch

Enter the number of the build you want to start and press enter

    Build the Code:

    time mka device

