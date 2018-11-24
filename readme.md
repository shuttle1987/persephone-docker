# Persephone docker deployment

This repository contains an automated deployment of the Persephone web stack including the web API and web frontend.
This uses docker-compose to run the various required docker images.

## Prerequisites

You need to have `docker-compose` installed.

See the [official install instructions](https://docs.docker.com/compose/install/)

Because the docker-compose.yml file specifies compose file format "3.0" you will need to have at least docker engine 1.13.0+.

For more information on minimum versions see the [Docker official compatibility page](https://docs.docker.com/compose/compose-file/compose-versioning/#compatibility-matrix)

## Running

To run use the following command:

```sh
docker-compose up
```

This will fetch the requisite images the persephone tools project has on Docker hub and will start them up.
