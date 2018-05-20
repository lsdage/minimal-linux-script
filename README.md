# Minimal Linux Script

One script which generates fully functional live Linux ISO image with minimal effort. This is a fork of [Minimal Linux Script](https://github.com/ivandavidov/minimal-linux-script).
The goal is to add USB 3 support in order to make a small system with DD for backups.

with some improvements taken from the next releases. All empty lines and comments have been removed and the script has been modified to reduce the overall length.

The script uses **Linux kernel 4.16.9**, **BusyBox 1.28.3** and **Syslinux 6.03**. The source bundles are downloaded and compiled automatically.

If you are using [Ubuntu 18.04](http://ubuntu.com), you should be able to resolve all build dependencies by executing the following command:

    sudo apt-get install wget bc build-essential gawk xorriso syslinux-utils bison flex libelf-dev libssl-dev

After that simply run the script:
    ./minimal.sh
    
It doesn't require root privileges. In the end you should have a bootable ISO image named `minimal_linux_live.iso` in the same directory.
