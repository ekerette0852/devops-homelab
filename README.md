![CI](https;//github.com/Ekerette0852/devops-homelab/actions/workflows/ci.yml/badge.svg)
![CD](https://github.com/Ekerette0852/devops-homelab/actions/workflows/cd.yml/badge.svg)

## published image
_ Proxy image published to Github Container Registry
- package: `ghcr.io/ekerette0852/devops-homelab/proxy:latest`
                                                              
# DevOps Homelab: Multi-service Reverse Proxy with Docker Compose

## Features
- Multi-service architecture (App1, App2)
- NGINX reverse proxy (path-based routing)
- Docker Compose orchestration
- CI pipeline with GitHub Actions
- CD pipeline publishing images to GitHub Container Registry

## Overview
This project demonstratea a simple DevOps architecture using Docker Compose and NGINX as a reverse proxy.

It routes traffic to multiple services using **path-based routing**.

## Architecture
- **NGINX Reverse Proxyy**
- **App1 (NGINX static site)**
- **App2 (NGINX static site)**
- **Docker Compose Networking**

## Traffic flow
Client -> NGINX Proxy -> App1 (/)
                         -> App2 (/app2/)

## Setup & Run
```bash
git clone https://github.com/Ekerette0852/devops-hhomelab.git
cd devops-homelab
sudo docker-compose up -d
```

## Access
- Main App -> http://localhost
- App2 -> http://localhost/app2/
