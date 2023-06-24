# Jenkins Agent Docker Container

This repository contains a Dockerfile for building a Jenkins agent container based on the `jenkins/inbound-agent` image.

## Prerequisites

- Docker should be installed on the host machine.

## Getting Started

To get started, follow the instructions below to pull and run the Jenkins agent container:

1. Clone this repository to your local machine:

```bash
docker pull giovannirossini/jenkins-agent:latest
```

## Container Details

The Jenkins agent container is based on the `jenkins/inbound-agent` image, version `3107.v665000b_51092-5`.

### Installed Packages

The following packages are installed in the container:

- apt-transport-https
- ca-certificates
- python3
- python3-pip
- curl
- wget
- zip
- unzip

### AWS CLI

The AWS Command Line Interface (CLI) is installed and upgraded to the latest version using pip3.

### Docker

Docker is installed in the container using the script obtained from `https://get.docker.com`. This allows the Jenkins agent to interact with Docker.

## Usage

Once the Jenkins agent container is up and running, it can be used as a build agent by connecting it to a Jenkins master. Refer to the Jenkins documentation for detailed instructions on how to configure and connect a Jenkins agent.
