# hugo-blowfish-production-example

## About

This repository provides an example of deploying a Hugo + Blowfish blog using Docker Compose, Nginx with PageSpeed, and Traefik.

### Features

- **Hugo**: A fast and flexible static site generator.
- **Blowfish**: A theme for Hugo.
- **Docker Compose**: Tool for defining and running multi-container Docker applications.
- **Nginx with PageSpeed**: High-performance web server with PageSpeed module for optimizing site performance.
- **Traefik**: A modern reverse proxy and load balancer.

As an example you can visit my blog at [sancholabs.com](https://sancholabs.com)

### Deployment

The deployment is divided into two stages:

1. **Development**: Uses `Dockerfile.development` to set up a local development environment with Hugo.
2. **Production**: Uses `Dockerfile.deployment` and `docker-compose-deploy.yml` to build and deploy the site with Nginx and Traefik.

### Files

- `Dockerfile.development`: Sets up the development environment.
- `Dockerfile.deployment`: Builds the production-ready site.
- `docker-compose.yml`: Defines the development services.
- `docker-compose-deploy.yml`: Defines the production services.

### Usage

#### Development

To start the development environment, run:


## Development

To generate the site run:

```bash
docker compose run --rm hugo new site .
