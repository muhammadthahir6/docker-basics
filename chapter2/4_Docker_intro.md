# Docker

+ is a software that packages app into standardized units called containers that have everything the app needs to run including libraries, system tools, code, and runtime.

## Components

+ Docker daemon, `dockerd`
    + a persistent process that manages Docker containers and handles container objects
+ Docker Client, `docker`
    + provides a command-line interface, CLI, that allows users to interact with Docker daemons via the Docker Engine API.

## Objects

+ Docker container
    +  a standardized, encapsulated environment that runs applications.
    + is managed using the Docker API or CLI.
+ Docker image
    + a read-only template used to build containers.
    + used to store and ship applications.
+ Docker service
    + allows containers to be scaled across multiple Docker daemons
    + result is known a `swarm`, a set of cooperating daemons that communicate through the Docker API.

## Docker Registries (docker hub)

+ a repository for Docker images.
+ private and public repos
+ can push and pull images

