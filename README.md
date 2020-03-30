![Logo of the project](https://raw.githubusercontent.com/mrlucasfreitas/easy-vagrant/master/img/vagrant01.png)

# Easy Vagrant
> Always in branch Master.

Welcome to my fast project about vagrant, easy, simple and functional.

My objective is to show vagrant for daily use in uncomplicated, simple and useful ways.

## Why use Vagrant?
Use mainly to learn, test and develop environments, because Vagrant is a manipulator of virtual machines that can be created, modified and destroyed with just one command (after configuring Vagrantfile).

In particular, I use it for software testing, application deployment and my favorite, creating ansible roles.

## Install Vagrant
Use the commands to install in MAC or Linux.

### Fisrt
Install VirtualBox from official [site](https://www.virtualbox.org).

### MacOS
After installing homebrew.
```sh
$ brew cask install vagrant
$ brew cask install vagrant-manager
$ vagrant --help
```

### Linux
```sh
$ apt update
$ apt install vagrant
```

## Basic commands
Now create a test directory and cd into the test directory.
Initialize the vagrant machine.
```sh
$ vagrant init precise64
```

Start the machine.
```sh
$ vagrant up
```

Show machine status.
```sh
$ vagrant status
```

You can ssh into the machine.
```sh
$ vagrant ssh
```

Reload the vagrant machine.
```sh
$ vagrant reload
```

Suspend the vagrant machine.
```sh
$ vagrant suspend
```

Active the machine that was suspended.
```sh
$ vagrant resume
```

Halt the vagrant machine.
```sh
$ vagrant halt
```

Destroy the vagrant machine.
```sh
$ vagrant destroy
```

## Vagrantfile examples
Some examples of Vagrantfile that can be used:

- [Basic](https://github.com/mrlucasfreitas/easy-vagrant/tree/master/samples/basic)

  _A basic configuration for starting a Vagrantfile._

- [Advanced]()

  _A more complete Vagrantfile configuration, containing array and loops._

- [Ansible](https://github.com/mrlucasfreitas/easy-vagrant/tree/master/samples/ansible-provision)

  _Automatically provisioning a Vagrant machine in an Ansible role._

- [Execute scripts](https://github.com/mrlucasfreitas/easy-vagrant/tree/master/samples/execute-script)

  _Run SH scripts on a Vagrantfile._

- [Kubernetes]()

  _Use for Kubernetes Cluster tests, you need good settings._

- [My Vagrant](https://github.com/mrlucasfreitas/easy-vagrant/tree/master/samples/my-vagrant)

  _My daily use, a mix of all the examples above._
  
## Additional informations

In this project, I used [Bento](https://app.vagrantup.com/bento)'s images, but feel free to change.

OS used:
- Ubuntu 18
- CentOS 6
- CentOS 7
- CentOS 8
- FreeBSD 12

Other images and versions available: [Vagrant Cloud](https://app.vagrantup.com/boxes/search)
