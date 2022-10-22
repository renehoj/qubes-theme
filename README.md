# qubes-theme
Plymouth theme for Qubes OS

this theme only allows you to use the luks password, if you are using any other type of authentication don't expect it to work.

# install
clone the repo and copy qubes-theme to /usr/share/plymouth/themes

check if the theme is avaiable, qubes-theme should be in the theme list
$ plymouth-set-default-theme -l

set the theme active
$ sudo plymouth-set-default-theme -R qubes-theme

# reinstall default theme
$ sudo plymouth-set-default-theme -R qubes-dark

# disaster recovery
if you system does boot disable plymouth, and and enable the default theme.

at the grub boot prompt use e to edit the boot config, add the following to the boot parameters

rd.plymouth=0 plymouth.enable=0
