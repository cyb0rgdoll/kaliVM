KaliVM - Cyb0rgdoll's Vagrant file version 1

This repository contains my vagrant file that spins up a Kali virtual machine on Virtual Box.

Configurable list of customizable modifications, tools & scripts includes:

 **   Changing "vagrant ssh" to use root
    Adding swap space
    Setting BASH aliases
    Adding extra wordlists
    Installing wine
    Update & dist-upgrade
    Prepping metasploit
    Cloning useful git repos like AutoBlue and AutoRecon etc
    Installing common exploit dependecies and mingw
    Setting up UFW
    Zsh (oh-my-zsh terminal shell)
    IntRec-Pack, Intelligence and Reconnaissance Package Installer (author: NullArray/Vector)
**
-- **Prerequisites** --

You'll need to have the following ready before you can use this:

**    VirtualBox 6 installed
    Vagrant 2.x installed**

-- **Installation instructions** --

Clone this repo by typing:
    
**`git clone https://github.com/cyb0rgdoll/kaliVM/`**
    
or simple download the Vagrantfile to a directory or folder of your own
    
Navigate to the directory, open Vagrantfile in your favorite editor to review/customize settings if need to
From Windows Command Prompt or command shell, start the Virtual machine by typing:
    
**   `vagrant up`**

The first time this runs will take some time doing provisioning and not require any further interaction. Vagrant will download the base Kali box,     configure the VM in virtualbox and run provisioning scripts. 

When ready, use Kali, login, change the root password and by using the command:
    
**  `sudo passwd root`**
    
When prompted enter your systems root command. If this is a fresh install of Kali, the default password will be set to 'kali' or 'vagrant'

**  `vagrant ssh`**

-- **Usage** --

You can use your VM headless or open the virtualbox gui and attach to the running vm to login with a graphical UI.
X11 forwarding is an option in the Vagrantfile for headless usage, easier if your host is linux.

#start virtual machine

**`vagrant up`**

#login

**`vagrant ssh`**

#stop the vm

**`vagrant halt`**

#when you want to start with a clean install
**
`vagrant destroy
vagrant up`**

