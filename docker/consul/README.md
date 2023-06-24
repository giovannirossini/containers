# Consul Docker Compose

This repository contains a `docker-compose.yaml` file for running Consul using Docker Compose.

## Prerequisites

- Docker and Docker Compose should be installed on the host machine.

## Getting Started

To get started, follow the instructions below to run Consul using Docker Compose:

1. Run the Docker Compose command to start Consul:

```bash
docker-compose up -d
```

This will start Consul in detached mode.

## Accessing Consul

Consul will be available at `http://localhost/`. You can access the Consul UI and interact with the server using this URL.

## Customizing ACL Configuration

To customize the ACL configuration, modify the `consul-acl.json` file in the `.data/config` directory. Restart the Consul container for the changes to take effect.

## Further Configuration

For advanced configuration options, refer to the [Consul documentation](https://www.consul.io/docs/agent/options) and modify the `docker-compose.yaml` file accordingly.
