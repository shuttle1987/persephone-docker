# Persephone docker deployment

This repository contains an automated deployment of the Persephone web stack including the web API and web frontend.
This uses docker-compose to run the various required docker images.

## Prerequisites

You need to have `docker-compose` installed.

See the [official install instructions](https://docs.docker.com/compose/install/)

Because the docker-compose.yml file specifies compose file format "3.0" you will need to have at least docker engine 1.13.0+.

For more information on minimum versions see the [Docker official compatibility page](https://docs.docker.com/compose/compose-file/compose-versioning/#compatibility-matrix)


### installing a newer docker-compose

If you are on Linux and have an out of date docker-compose we suggest installing it as a user package suing pip.

First create a virtualenvironment:

```sh
$ python3 -m venv venv
$ source venv/bin/activate
(venv) $ pip install -U pip
```

Then install docker-compose via pip:

```sh
(venv) $ pip install docker-compose
```

Check if this has worked with:

```sh
(venv) $ docker-compose --version
docker-compose version 1.23.1, build b02f130
```

## Running

To run use the following command:

```sh
docker-compose up
```

This will fetch the requisite images the persephone tools project has on Docker hub and will start them up.

### Updates

The Docker images are regularly updated, if your images get out of date you can update them to the most recent version with:

```sh
docker-compose pull
```
