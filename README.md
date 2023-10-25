# Setup Arch Linux machine using Arch Installer

## Initial configuration of installer 

> # iwctl
> \[iwd\] device list
> \[iwd\] station wlan0 scan
> \[iwd\] station wlan0 connect GALILEE
> password: KashmirRemy
> \[iwd\] station wlan0 show
> \[iwd\] exit
> # ping archlinux.org
> # timedatectl
> # archinstall

## Installation using Archinstall
Use xfce window manager (use full desktop option); use network-manager to manage network
Extra packages: git ansible ansible-core lazygit network-manager-applet

## Reboot

## Setup configuration
### Log in using xfce window manager
### > git clone https://github.com/rickprice/dotfiles .dotfiles
### > git clone https://github.com/rickprice/AAConfig

## Setup computer using Ansible
> ansible-galaxy collection install -r requirements.yml
> ansible-playbook --ask-become-pass --connection=local setup_computer_basic.yml

## Setup computer using dotter
### Checkout the correct branch for the computer being setup_computer
### Run dotter
### in XMonad configuration directory
> git submodule init
> git submodule update --remote
> xmonad --recompile
