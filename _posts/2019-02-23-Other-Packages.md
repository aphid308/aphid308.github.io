---
layout: post
title: Other Packages and Exa
---
#### Other Packages
__These are some other packages that my environment uses__  
```bash
sudo apt-get install -y tmux virtualenv \
                        virtualenvwrapper python3-pip \
                        libffi-dev libssl-dev \
                        libjpeg-dev libpq-dev \
                        postgresql
```
#### Exa
_exa is a replacement for ls that implements better visual cues, tree visualization and git status integration_  
__Install Rust using Rustup__  

```bash
curl https://sh.rustup.rs -sSf | sh
sudo apt-get install -y cargo libgit2-26
sudo apt-get install -y libgit2-26
```
__Install Exa__  
_I compile exa from source because it's pretty easy and they do not have a .deb package available for download_  
```bash
git clone https://github.com/ogham/exa.git
cd exa
sudo make install
```
#### Exa in action
<script id="asciicast-229426" src="https://asciinema.org/a/229426.js" async></script>
<iframe src='https://gfycat.com/ifr/UntimelyDeliciousIriomotecat' frameborder='0' scrolling='no' allowfullscreen width='640' height='489'></iframe>
