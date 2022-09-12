# Simple Monerod Docker

A simple and straightforward Dockerized [MoneroBlock](https://github.com/duggavo/MoneroBlock) built from source and exposing standard ports.

## Actions

[![Weekly Update Rebuild](https://github.com/sethforprivacy/moneroblock-docker/actions/workflows/update-base-image.yml/badge.svg)](https://github.com/sethforprivacy/moneroblock-docker/actions/workflows/update-base-image.yml)  
[![Latest Dockerfile build on push](https://github.com/sethforprivacy/moneroblock-docker/actions/workflows/update-image-on-push.yml/badge.svg)](https://github.com/sethforprivacy/moneroblock-docker/actions/workflows/update-image-on-push.yml)  

## Docker

![Docker Pulls](https://img.shields.io/docker/pulls/sethsimmons/moneroblock)  
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/sethsimmons/moneroblock/latest)  
![Docker Image Version (latest by date)](https://img.shields.io/docker/v/sethsimmons/moneroblock)  

## Docker Hub

This repo is used to build the images available at:

https://hub.docker.com/r/sethsimmons/moneroblock

## Tags

`latest`: The latest branch version of MoneroBlock from https://github.com/duggavo/MoneroBlock, built on an Alpine base image  
`branch_name`: The version corresponding with the branch from https://github.com/duggavo/MoneroBlock, built on an Alpine base image  

## Recommended usage

The ways I would generally recommend running this container for a personal or public Monero explorer are below.

MoneroBlock explorer using a public node:

```bash
sudo docker run -d --restart unless-stopped --name="moneroblock" sethsimmons/moneroblock:latest --daemon node.sethforprivacy.com:18089
```

Ideally you will run your own instance of `monerod` and point MoneroBlock to it.

## Copyrights

Code from this repository is released under MIT license. [@duggavo License](https://github.com/duggavo/MoneroBlock/blob/main/license.txt)
