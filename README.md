# gatling-nginx-tool

## Overview

It is a tool that provides gatling(v3.2.0) and nginx containers, and you can stress test as soon as you have a scenario file.

## Requirement
* docker
* docker-compose

## Usage

* start the container with docker-compose
```
docker-compose up -d --build
```

* run a stress test, and choose the scenario file.
```
docker exec -it `docker ps --filter name=gatling --format "{{.ID}}"` /usr/local/bin/gatling/bin/gatling.sh
```

you can check the result file tree by accessing `http://localhost/`

## Features
* The result file is persisted to the `./result` in the project root directory.
