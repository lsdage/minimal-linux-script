# Minimal Linux Script

This is a fork of [Minimal Linux Script](https://github.com/ivandavidov/minimal-linux-script): One script to generate a minimalistic live Linux ISO image.

The goal of this fork is to have USB 3 support in order to make a miniature system with DD for backups.

The script uses **Linux kernel 4.17.3**, **BusyBox 1.28.4** and **Syslinux 6.03**. The source bundles are downloaded and compiled automatically.

On [Ubuntu](http://ubuntu.com), the following command should resolve all build dependencies:

    sudo apt-get install wget bc build-essential gawk xorriso syslinux-utils bison flex libelf-dev libssl-dev

After that simply run the script:

    ./minimal.sh

The script doesn't require root privileges. In the end there should be a bootable ISO image named `minimal_linux_live.iso` in the same directory.
