# Docker Workshop

## Installation

Git clone [https://github.com/Niloc91/docker-ng-example](https://github.com/Niloc91/docker-ng-example)

Git clone [https://github.com/Niloc91/kotlinexample](https://github.com/Niloc91/kotlinexample)

Docker  from dockerhub : [https://docs.docker.com/docker-for-mac/install/](https://docs.docker.com/docker-for-mac/install/)

Jdk8

Angular cli tool

## Why do we use docker?

- Packaging and deploying
- Easier to share
- Speed of development

## Knowledge (that will be hopefully acquired)

- How to interact with dockerhub
- How to pull and push images
- How to create a simple dockerfile
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

### Dockerhub account

Create a dockerhub account: http://dockerhub.com

### Login

Login to dockerhub using your account details

### Pull, retag and push

Using commands above pull nginx image locally, retag the image and push to your container repo.

### Dockerfile

Write a simple Dockerfile to replace the default nginx page with a hello world page

### Tag and push new image

Retag and push dockerfile to your account

### Pairs, build and share

FE: clone [https://github.com/Niloc91/docker-ng-example](https://github.com/Niloc91/docker-ng-example)

BE: clone [https://github.com/Niloc91/kotlinexample](https://github.com/Niloc91/kotlinexample)

FE: Clone repo, build angular project, push to container repo and provide instructions for BE to pull and run

BE: Same as above

### Docker-compose

Using configuration above have both images running 2 instances of BE and FE.

FE should be served on ports 80 and 81

BE should be served on ports 8080 and 8081

### Configuration changes
Configure from docker-compose file, the index.html on the FE instance to switch between the 2 backend instances without rebuilding the image. 


# 
