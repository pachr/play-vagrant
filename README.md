#Play framework and Vagrant with some Ansible magic

A simple Vagrant config with Play Framework, Ansible and MySQL server that gets you started quickly with a working example. When deployed, the folder structure will look like this: 
- yourrepo/
  - frameworks/
      - activator-1.3.10-minimal/
  - project/
      - (We will clone & pull our project repo here)
  - provision/
      - templates/
      - ansible_hosts
      - playbook.yml
  - ansible.cfg
  - Vagrantfile


##Requirements

On your machine, install everything listed below: 

- GIT, Java, ... the basic stuff
- VirtualBox https://www.virtualbox.org/
- Vagrant http://www.vagrantup.com/  (ATOW version 1.4.3)
- Ansible http://docs.ansible.com/ (ATOW version 1.5)
- Some console knowledge :-)

##Getting Started

  Anywhere on your machine
    
  ```bash

    $> git clone git@github.com:pachr/play-vagrant.git yourrepo && cd yourrepo && vagrant up

  ```  
  *Note : Change yourrepo to something good*

This takes time. Grab a beer :beer: - or two! :beers:

  Then

  ```bash

    $> vagrant ssh

  ```    

  Your vagrant box is up and running !


We will see how to download our project after  

~~When it's ready, go to your browser and enter http://localhost:9000/~~
~~Le voilà!~~

##Tips and tricks

- If the filesystem is slow, set NETWORK_FILE_SYSTEM to true in the Vagrantfile, reboot the VM ("vagrant halt; vagrant up") and enter your root password.

##Problems?

Vagrant and ansible have good dokumentation at http://docs.vagrantup.com/v2 and http://docs.ansible.com/

[Thanks to torbjokv](https://github.com/torbjokv/play-vagrant)
