# docker_installation_in_5

This is to install the latest docker on Ubuntu 20.04 LTS version with one shell script. To install the latest docker

Prerequisites:
  1. edit visudo to all the docker installation user no password for sudo
  2. install git
    $ sudo apt install -y git
  3. git clone https://github.com/morriswangx/docker_installation_in_5.git

Installation:
  1. $ sudo apt-get update
  2. $ cd docker_installation_in_5
  3. chmod +x docker_install.sh
  4. ./docker_install.sh

To verify your installation:
  $ docker images     // you shall not see any images
  $ docker run hello-world    // this will pull  a hello-world image from docker hub and run it
  $ docker ps           // hello-world container is running.
  
To delete docker:
  1. stop the container(s)
  2. delete the container(s)
  3. delete the images
  4. $ sudo apt-get purge docker-ce docker-ce-cli containerd.io docker-compose-plugin
