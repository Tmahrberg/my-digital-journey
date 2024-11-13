---
{"dg-publish":true,"permalink":"/my-digital-journey/homelab/docker/"}
---

I run mostly everything using Docker.
So here i will tell you how to install and get it going!

First setup Docker's apt repository.

> sudo apt-get update
> sudo apt-get install ca-certificates curl gnupg
> sudo install -m 0755 -d /etc/apt/keyrings
> curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
> sudo chmod a+r /etc/apt/keyrings/docker.gpg



### Add the repository to Apt sources:

> echo \
>   "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
>   "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
> sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
> sudo apt-get update

If you use an Ubuntu derivative distro, such as Linux Mint, you may need to use `UBUNTU_CODENAME` instead of `VERSION_CODENAME`._


##### Install the latest version

> sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin


##### Check installed version

> docker -v

##### Check docker compose

> docker compose

##### Check runtime

> sudo docker run hello-world


## Use Docker without sudo

> sudo usermod -aG docker  $USER

You'll need to logout then back in to apply this.


### Cleaning Up

If you need to uninstall docker, run the following

> sudo apt-get purge docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin docker-ce-rootless-extras




[[My Digital Journey/Homelab/My software of choice!\|My software of choice!]]


