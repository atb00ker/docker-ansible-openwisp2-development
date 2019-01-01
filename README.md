# docker-ansible-openwisp2-development

This repository is for development only not the end-user.

[![Build Status](https://travis-ci.org/atb00ker/docker-ansible-openwisp2-development.svg?branch=master)](https://travis-ci.org/atb00ker/docker-ansible-openwisp2-development)
[![Docker Hub](https://img.shields.io/badge/docker--hub-atb00ker%2Fansible--openwisp2--development-brightgreen.svg)](https://hub.docker.com/r/atb00ker/ansible-openwisp2-development)
[![GitHub](https://img.shields.io/badge/github-docker--ansible--openwisp2--development-brightgreen.svg)](https://github.com/atb00ker/docker-ansible-openwisp2-development)


## Image tags

- Debian: `debian10`, `debian9`, `debian8`
- Fedora: `fedora26`, `fedora27`, `fedora28`
- Ubuntu: `ubuntu16`, `ubuntu18`
- CentOS: `centos6`, `centos7`

## Usage

```console
$ docker network create --driver bridge --subnet <network_address> --gateway <gateway_address> docker-bridge
$ docker run -dit --privileged --name "$current_name" --net docker-bridge --ip=$current_ip atb00ker/ansible-openwisp2-development:<image-tag>
```
Example values:
```
<network_address>: 192.168.56.33/27
<gateway>: 192.168.56.33
<ipadress>: 192.168.56.35
```

## Container login information

- user: root
- password: root

Feel free to open an issue and talk about the repository.