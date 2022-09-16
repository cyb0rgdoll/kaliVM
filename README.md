This rep contains my vagrant file that spins up a Kali virtual machine (using Virtual Box) 
with a configurabe list of customizable modifications such as:

    changing "vagrant ssh" to use root
    adding swap space
    setting BASH aliases
    adding extra wordlists
    installing wine
    update & dist-upgrade
    prepping metasploit
    cloning useful git repos like AutoBlue and AutoRecon etc
    installing common exploit dependecies and mingw
    setting up UFW
    zsh (oh-my-zsh terminal shell)

Prerequisites

You'll need to have the following ready before you can use this:

    VirtualBox 6 installed and working
    Vagrant 2.x installed and working

Installing

    Clone this repo or simple download the Vagrantfile to a directory
    Navigate to the directory, open Vagrantfile in your favorite editor to review/customize settings if needed
    From a command shell, start the VM. The first time this runs will take some time doing provisioning.
    
    vagrant up

    Vagrant will download the base Kali box, configure the VM in virtualbox, run provisioning scripts. 
    The first time this runs this can take some time but should not require any interaction.

    Login, change the root password and use Kali

    vagrant ssh

Usage

You can use your VM headless or open the virtualbox gui and attach to the running vm to login with a graphical UI.

X11 forwarding is an option in the Vagrantfile for headless usage, easier if your host is linux.


#start vm

vagrant up

#login

vagrant ssh

#stop the vm

vagrant halt

#when you want to start with a clean install

vagrant destroy
vagrant up

