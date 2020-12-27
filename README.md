# pacrep
Choose pacman repositories on a per package basis

# Description

This script takes basically two options: -a, to update and upgrade the entire system, and -s, to install single packages. Once it knows what is to be installed/upgraded, it checks everything against a rules list (a series of lines in the form repo/pkg defined in the configuration file), and, if a rule for the package is found, installs the package from the specified repository (instead of from the first repository defined in `/etc/pacman.conf` providing the package, which is pacman's default behaviour).

The main idea of this script is to make pacman able to handle packages with the same name in different repositories, for example, core/licenses and libre/licenses. Just define in the configuration file from which repository is package is to be installed and pacman will always install/upgrade the package from the specified repository (disregarding the repositories order in `/etc/pacman.conf`).
