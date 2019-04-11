# dockerworkshop2

## Installation

Git clone [https://github.com/Niloc91/docker-ng-example](https://github.com/Niloc91/docker-ng-example)

Git clone [https://github.com/Niloc91/kotlinexample](https://github.com/Niloc91/kotlinexample)

Docker  from dockerhub : [https://docs.docker.com/docker-for-mac/install/](https://docs.docker.com/docker-for-mac/install/)

Jdk8

Angular cli tool

## App/Builder pattern why?

- Allows other developers to modify and build
- Reduces final image size
- No need for build tools to be installed locally

## Knowledge (that will be hopefully acquired)

- Creation of builder and app images
- Passing files between images
- Using helper scripts
- Orchestration with docker-compose

## Helpful commands

- `**docker pull** <container repo>/<image name>:<tag> (pull image from container repo)`
- example – `docker pull nginx:15.9-alpine` (no need to specify repo as from dockerhub)
- `**docker tag** <old tag> <new tag>` (used to tag images, generally used to tag and pushto a new container repo)
- `**docker login** -u <username>`
- `**docker push** <container repo>/<image name>`
- `**docker ps**`
- `**docker build** -t <image name> -f <path to dockerfile> <build context>`
- example – `docker build -t local/exampleapp -f Dockerfile .`
- `**docker images**`

## Exercises

### Refresher
Create build and upload to dockerhub a custom website with "Hello Dockerhub" packaged on an Nginx image.

### Create github account
Create a github account with the project and any tools associated

### Create angular project/java project
Create a sample project with the language of your choice to run locally. Ideally  

### App/Builder dockerfiles
Create 2 docker files in different folders one containing the 
build tools for the project and the second containing whats needed
to run the project.

### Helper scripts
Create helper scripts to build the project e.g. Bash, Makefile etc.

### Push changes to github
Push all changes along with instructions to build and run the project, the developers building the project
should not need any of the local build tools installed.

### Debugging
The last exercise will be debugging a bad build.

Clone the repository below.
https://github.com/Niloc91/docker-ng-example
