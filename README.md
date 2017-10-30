# tbrowet/docker-sslscan

[sslscan](https://github.com/rbsec/sslscan) in a container.

## Requirements

* [Docker](https://www.docker.com/)

## Installation

Get the [trusted build on the docker hub](https://registry.hub.docker.com/u/tbrowet/docker-sslscan/):

```bash
$ docker pull ThomasBrowet/docker-sslscan
```

or download and compile the source yourself from Github:

```bash
$ git clone https://github.com/tbrowet/docker-sslscan.git
$ cd docker-sslscan
$ docker build -t ThomasBrowet/docker-sslscan .
```

## Usage

It tests SSL/TLS enabled services to discover supported cipher suites.

Example usage:

```bash
$ docker run --rm ThomasBrowet/docker-sslscan www.google.com
```