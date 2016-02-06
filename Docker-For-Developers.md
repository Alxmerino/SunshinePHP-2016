# Docker For Developers

###Chris Tankersly | @dragonmantank | https://github.com/dragonmantank/dockerfordevs-app

* * *


## Some notes

* -p [local port]:[container port] - local port is only needed if it needs to go through the host, if container only need to talk to each other only container port is necessary

* docker generally runs as root on containers, which sometimes creates permission issues

* Not recommended to run more than one process per container

## Docker Links

* Allows containers to `see` each other over network

* Containers must live on the same host

* `--link` [container name]:[internal name]

## Docker Swarm

* Cluster management tool developed by Docker

* Looks like a machine running Docker but is actually multiple machines

* Volumes on Swarm cannot be shared across hosts

## Docker Compose

* Multi-container orchestration

* A single config gile holds all of your container info

* works with Docker Swarm and a few other tools, like Rancher

    * `docker-compose.yml - Uses yaml

* Does not work with Swarm

## Deploying

* `Rancher` is a good start

* provides a nice GUI to manage everything

* Allows volume sharing and networking across hosts

* Works with docker-compose.yml files

http://ctankersley.com

[chris@ctankersley.com](mailto:chris@ctankersley.com)

https://joind.in/talk/c1ecb

