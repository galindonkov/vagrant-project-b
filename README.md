### Description

A project that creates two ```vagrant boxes``` using single Vagrant file.

### Installed softwares needed prior to using the project

- VirtualBox software installation : [link for VirtualBox](https://www.virtualbox.org/wiki/Downloads)

- Vagrant software installation : [link for Vagrant](https://www.vagrantup.com/docs/installation/)

### The repo is having following files

- File ```Vagrantfile``` : Has the configuration for vagrant, about what type of VM we want, once set, executing vagrant up will have our clean environment

### How to use the repo

- Clone this repo to your local machines : `git clone git@github.com:galindonkov/vagrant-project-b.git`

- Change to the currently added directory : `cd vagrant-project-b/`

- Execute `vagrant up` to build your local DEV environments

- Once the DEV environments are created, list to check them by : ```vagrant status``` and the result will be :
```
Current machine states:

web01                     running (virtualbox)
web02                     running (virtualbox)
```

- Above output is a proove that both virtual machines ```web01 and web02``` are created successfully and you can connect either to web01 by ```vagrant ssh web01``` or to web02 by ```vagrant ssh web02```

- Once you finish with the test type `exit` to leave the Vagrant-built virtual machine.

- Bear in mind that the Vm will remain running, so in case it is not needed anymore you can either shut down the running machine Vagrant is managing by `vagrant halt` or using `vagrant destroy` to stop the running machine and destroy all resources that were created during the machine creation process.
