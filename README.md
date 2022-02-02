# My datascience notebook

To build a custom docker image, make sure that the "Dockerfile" text file with the docker script called in the docker build argument. It can be called with a file path or with a "." if you're already in the file.

##Image Link
My image is hosted on [Dockerhub](https://hub.docker.com/repository/docker/dylanbolt/my-datascience-notebook)

##How to use image with docker compose
Make sure that the image is tagged to dylanbolt/my-datascience-notebook. Under build simply put "." so that it looks in the locak directory.
