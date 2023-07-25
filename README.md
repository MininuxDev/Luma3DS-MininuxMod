# Why this fork
I initially used the [Luma 10.3 with Night/Light and Quick-Switchers](https://gbatemp.net/download/luma-10-3-with-night-light-and-quick-switchers.35619/) mod by DullPointer, but it was on 10.3 and i wanted to use the latest Luma v13. But there are some features from the Quick-Switchers fork that I absolutely needed, for example toggling wifi with START on rosalina menu (very handy on n3DS). I also noticed there were some rejected pull requests on the official Luma3DS repo. I've never programmed anything for consoles, nor anything significant in C, but the code was simple enough that i could merge and customize some stuff.

I insist, **i've never programmed anything for consoles**, so maybe i'm doing wrong and buggy stuff. Although the changes i added for the moment are pretty innofensive, keep backups in case something goes wrong (it won't be my fault :)

# Added functionnality
* Start button toggles WIFI on rosalina menu ([from the Quick Switchers fork by DullPointer](https://github.com/LumaTeam/Luma3DS/commit/c1a20558bed3d792d54069719a898006af20ba85))
* IP address always shown on rosalina menu ([original PR by ReplayCoding](https://github.com/LumaTeam/Luma3DS/pull/1282/commits/35f6ab10c9e5240d0a64bc09c335ed06bc00f700))


# Now the Original Readme

# Luma3DS
*Noob-proof (N)3DS "Custom Firmware"*

### What it is
**Luma3DS** is a program to patch the system software of (New) Nintendo (2)3DS handheld consoles "on the fly", adding features such as per-game language settings, debugging capabilities for developers, and removing restrictions enforced by Nintendo such as the region lock.

It also allows you to run unauthorized ("homebrew") content by removing signature checks.
To use it, you will need a console capable of running homebrew software on the Arm9 processor.

Since v8.0, Luma3DS has its own in-game menu, triggerable by <kbd>L+Down+Select</kbd> (see the [release notes](https://github.com/LumaTeam/Luma3DS/releases/tag/v8.0)).

#
### Compiling
* Prerequisites
    1. git
    2. [makerom](https://github.com/jakcron/Project_CTR) in PATH
    3. [firmtool](https://github.com/TuxSH/firmtool)
    4. Up-to-date devkitARM+libctru
1. Clone the repository with `git clone https://github.com/LumaTeam/Luma3DS.git`
2. Run `make`.

    The produced `boot.firm` is meant to be copied to the root of your SD card for usage with Boot9Strap.

#
### Setup / Usage / Features
See https://github.com/LumaTeam/Luma3DS/wiki

#
### Credits
See https://github.com/LumaTeam/Luma3DS/wiki/Credits

#
### Licensing
This software is licensed under the terms of the GPLv3. You can find a copy of the license in the LICENSE.txt file.

Files in the GDB stub are instead triple-licensed as MIT or "GPLv2 or any later version", in which case it's specified in the file header.
