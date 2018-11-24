# Persephone docker deployment

This repository contains an automated deployment of the Persephone web stack including the web API and web frontend.
This uses docker-compose to run the various required docker images.

## Prerequisites

You need to have `docker-compose` installed.

See the [official install instructions](https://docs.docker.com/compose/install/)

## Running

To run use the following command:

```sh
docker-compose up
```

This will fetch the requisite images the persephone tools project has on Docker hub and will start them up.
