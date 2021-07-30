Docker
#Install the yum-utils package (which provides the yum-config-manager utility) and set up the stable repository.
sudo yum install -y yum-utils  device-mapper-persistent-data  lvm2

sudo yum-config-manager  --add-repo   https://download.docker.com/linux/centos/docker-ce.repo

#if we have an error
sudo yum erase podman buildah

#install
sudo yum install docker-ce docker-ce-cli containerd.io

#start daemon
sudo systemctl start docker

#version
docker --version

#Set the boot
sudo systemctl enable docker

#test
sudo docker run hello-world