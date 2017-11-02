# ThomasBrowet/docker-sslscan

[sslscan](https://github.com/rbsec/sslscan) in a container.

## Requirements

* [Docker](https://www.docker.com/)

## Installation

Get the [trusted build on the docker hub](https://registry.hub.docker.com/u/tbrowet/docker-sslscan/):

```bash
$ docker pull thomasbrowet/docker-sslscan
```

or download and compile the source yourself from Github:

```bash
$ git clone https://github.com/thomasbrowet/docker-sslscan.git
$ cd docker-sslscan
$ docker build --rm -t thomasbrowet/docker-sslscan .
```

## Usage

It tests SSL/TLS enabled services to discover supported cipher suites.

Example usage:

```bash
$  docker run -it --rm thomasbrowet/sslscan www.google.com
```