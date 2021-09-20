# Docker
### Install the yum-utils package (which provides the yum-config-manager utility) and set up the stable repository.
```
sudo yum install -y yum-utils  device-mapper-persistent-data  lvm2

sudo yum-config-manager  --add-repo   https://download.docker.com/linux/centos/docker-ce.repo
```
### if we have an error
```
sudo yum erase podman buildah
```
### install
```
sudo yum install docker-ce docker-ce-cli containerd.io
```

### start daemon
```
sudo systemctl start docker
```

### version
```
docker --version
```

### Set the boot
```
sudo systemctl enable docker
```

#### test
```
sudo docker run hello-world
```
### Docker download image
Docker pull *name image*

### Build image
```
docker build .
docker images
docker run IMAGE_ID
docker ps -a
docker stop CONTAINER_ID
docker run -p -d 3000:3000 IMAGE_ID
```