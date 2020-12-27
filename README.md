# pacrep
Choose pacman repositories on a per package basis

This script grabs what is to be installed/upgraded, check it against a rules list (a series of lines in the form repo/pkg), and, if a rule for the package is found, installs the package from the specified repository (instead of from the first repository defined in `/etc/pacman.conf` providing the package, which is pacman's default behaviour).
