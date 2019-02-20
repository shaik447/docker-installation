# Docker Tutorials

This repo contains the code examples from my blog https://idevops.online/

# Docker Installation on Ubuntu
Run the following commands in sequence
```
$ sudo apt-get update
$ sudo apt install apt-transport-https ca-certificates curl software-properties-common
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
$ sudo apt-get update
$ sudo apt-get install docker-ce

```
After installation check the docker status and enable it to run on system startup
```
$ sudo systemctl status docker
$ sudo systemctl enable docker

```
# Run docker command without sudo
```
$ sudo usermod -aG docker ${USER}
```
Finally logout or restart for changes to take effect.

# Run a container to test the installation
```
$ docker run hello-world
```
This command downloads a test image and runs it in a container. When the container runs, it prints an informational message and exits.



