# Developer's VM
Development environment for developers (Tomcat : Fedora-Commons, Solr, Cocoon)

## Requirements
* [Packer](https://packer.io/) (Only for .box creation)
* [Vagrant](https://www.vagrantup.com/)
* [VirtualBox](https://www.virtualbox.org/)

## Usage

1. `git clone https://github.com/eruditorg/vm-dev.git`
2. `cd vm-dev`
3. `vagrant up`

You can use the GUI or you can also shell into the machine with `vagrant ssh`

## Environnement

* CentOs 7
  * Tomcat 7.0.54
    * Manager username: admin password: admin
  * Mariadb
    * Username: root Password: root
    * Database: fedora
      * Username: fedoraAdmin Password: fedoraAdmin
  * Fedora-Commons 3.4.2
    * Username: fedoraAdmin Password: fedoraAdmin
  * Solr 4.10.3
  * Eclipse Mars

## Base Commands

- vagrant up
  - Start the VM
- vagrant halt
  - Stop the VM
- vagrant provision
  - Run any configured provisioner configured in the Vagrantfile
- vagrant suspend
  - Stop the VM and save state
- vagrant ssh
  - Ssh into the running Vagrant machine
- vagrant destroy
  - Stop the VM and delete all traces


## Windows User

If you want to use **vagrant ssh** you will need git or cygwin.

  * [Git](https://git-scm.com/downloads)
  * [Cygwin](https://cygwin.com/install.html)
