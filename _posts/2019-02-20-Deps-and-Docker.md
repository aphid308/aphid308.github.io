--
layout: post
title: Installing Dependencies, Docker CE, and Docker Compose
--

### Install Dependencies
```bash
sudo apt-get install -y tmux virtualenv \
                        virtualenvwrapper python3-pip \
                        libffi-dev libssl-dev \
                        libjpeg-dev libpq-dev \
                        postgresql
```

### Install Docker CE
_Remove any old versions_

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```

_Install packages to allow for apt installation over https_

```bash
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent \
software-properties-common
```

_Add the Docker GPG key_

```bash
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

_Add the repository and specify the branch_

```bash
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
```

_Update the repo and install latest version of Docker CE and containerd_

```bash
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
```


