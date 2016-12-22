# cg-ng-idevice - Crosstool-NG iDevice Configuration

This repository contains the configuration necessary to build a iDevice
cross-compiling toolchain. It is based off of the arm-elf ct-ng
template, and adds some patches to make compiling work.

Note that this was generally made for older iDevices
(iPhone/iPod 1G/2G/3G). It does not target specific architectures, and
was created for assembling ARM instructions. Your mileage may vary if
you are using this toolchain for other purposes!

# Instructions

  1. Install the latest Crosstool-NG. These configuration files and
     builds were developed and tested with Crosstool-NG v1.22.0.

  2. Once installed, clone this repository to a place with lots of
     space. The build itself takes up around 4-5 GBs, and components
     can take up even more space.
     
     You should have at least 5 GBs of free space for your build, and
     5 GBs of free space for your installation (defaulting to home
     directory).

  3. Enter this repository's directory.

  4. (OPTIONAL) Configure your build with `ct-ng menuconfig`. By
     default, this toolchain installs to `$HOME/x-tools`. If you
     would like to change this, make sure to configure your build!

  5. Run `ct-ng build` to build and install your toolchain!

# Contributions
Contributions are always welcome! If you have any issues or fixes,
please let me know via GitHub!

# License
Note that this license only applies to the configuration - the
resulting compiled toolchain (and the resulting programs built from
it) does not apply here!

    Crosstool-NG iDevice Configuration
    Copyright (C) 2016 Albert Huang

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
