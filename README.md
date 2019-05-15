To setup docker on a linux machine follow the following steps


DOCKER
1.
sudo apt-get install \\
apt-transport-https \\
ca-certificates \\
curl \\
gnupg-agent \\
software-properties-common

2. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
3. sudo apt-key fingerprint 0EBFCD88
4. sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu\
 bionic stable"
5. sudo apt update
6.sudo apt install docker-ce docker-ce-cli containerd.io

DOCKER-MACHINE
1. base=https://github.com/docker/machine/releases/download/v0.16.0 &&\
  curl -L $base/docker-machine-$(uname -s)-$(uname -m) >/tmp/docker-machine &&\
  sudo install /tmp/docker-machine /usr/local/bin/docker-machine

Install virtual box

Change system bios to allow vitualization

Create docker machine instance
1. docker-machine create --driver virtualbox default

test

