# Mini Bootcamp image

This repository will create Vagrant box for mini bootcamp purpose

## Requirements
 - Working installation of [Vagrant](https://www.vagrantup.com/downloads)
 - Working installation of [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
 - Instance with virtualization capability and [VirtualBox](https://www.virtualbox.org/wiki/Downloads) installed

## Usage:
 1. Clone this repository
 1. In this repository, run `vagrant up`
 1. Access the instance with `vagrant ssh`
 1. File in this repository will be in sync with `/vagrant` in the VM

## Vagrant Commands
 - Start VM: `vagrant up`
 - Hibernate VM: `vagrant suspend`
 - Restart VM: `vagrant reload`
 - Destroy VM: `vagrant destroy`
