# docker-compose

## About

This repository contains the backups of all the docker-compose files I use for my personal home server.

## Tech stack

My server is currently running on a Lenovo Mini-PC with Fedora Server as the OS. Docker containers are managed using Portainer.

## Upgrading Portainer

- `docker stop portainer`

- `docker rm portainer`

- `docker run -d -p 8000:8000 -p 9443:9443 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:lts`

Read more: [documentation](docs.portainer.io/start/upgrade/docker)
