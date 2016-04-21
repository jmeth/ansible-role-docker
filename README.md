# Ansible Role :: Docker
---

This is a role for installing docker-engine and docker-compose on CentOS 7. Installation is done manually rather than using Docker's install scripts or docker-machine.  This is useful for custom deployments, production systems, and/or hosts requiring a specific release of docker.

## Requirements
* Ansible >= 2.0
* CentOS >= 7.2

## Versions
* docker: 1.9.1
* docker-compose: 1.5.2

## Role Variables
Available variables are listed below and configured in the defaults/main.yml file to allow for customization using Ansible variable precedence

```
docker_url: https://get.docker.com/builds/Linux
docker_version: 1.9.1
docker_group: docker
docker_port: 2375
docker_compose_url: https://github.com/docker/compose/releases/download
docker_compose_version: 1.5.2
bridge_ip: 172.17.0.1
```