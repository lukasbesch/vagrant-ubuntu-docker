# Ubuntu for docker development
Vagrantfile to provision Ubuntu with Docker and Docker Compose

## Why would I need that?

If you are on macOS, you have several options to use Docker:
  - You can use [Docker Toolbox](https://www.docker.com/products/docker-toolbox) with `docker-machine` to create an isolated docker environment with the [boot2docker](http://boot2docker.io/) image. Unfortunately you cannot use docker-compose from within.
  - You can use [Docker for Mac](https://www.docker.com/products/docker#/mac). Unfortunately you cannot SSH into the machine.

To overcome these drawbacks we have a fully fledged virtual machine running Ubuntu which runs docker.
Additionally, you don't need to have docker installed on your host machine. Of course, you will need [Vagrant](https://www.vagrantup.com/) and [Parallels (Pro or Business)](http://www.parallels.com/de/products/desktop/) and the [Parallels plugin for Vagrant](https://parallels.github.io/vagrant-parallels/).
If you do not have Parallels, try changing the base image to the default Ubuntu 14.04 image `ubuntu/trusty64`.
