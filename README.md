# basic-development-machine
development machine, contains Java8, IntelliJ IDEA, Git.

## client versions

- os: xubuntu-16.04
- java: 8
- idea: 2016.2.4
- git: 2.7.4
- apache: 2.4.18

## host environment requirement(recommended)

- vagrant: 1.8.5
- virtualbox: 5.0.18

- vagrant-vbguest
- vagrant-omnibus

## how to use

```bash
$ git clone https://github.com/akzero53/basic-development-machine.git
$ vi Vagrantfile # configure your setting
$ vagrant up --provider virtualbox --provision
```
