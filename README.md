
# My datascience notebook

To build a custom docker image, make sure that the "Dockerfile" text file with the docker script called in the docker build argument. It can be called with a file path or with a "." if you're already in the file.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DylanBolt/my-datascience-notebook/HEAD)

My image is hosted on [Dockerhub](https://hub.docker.com/repository/docker/dylanbolt/my-datascience-notebook)

## Using this repo
### With `docker`
Build:

```bash
 docker build --rm -t jupyter/my-datascience-notebook .
# To build a custom docker image, make sure that the "Dockerfile" text file with the docker script called in the docker build argument. It can be called with a file path or with a "." if you're already in the file.
```

Run:

```bash
docker run --rm -it -p 8888:8888 jupyter/my-datascience-notebook
# - Should publish port 8888
# - Should mount the local directory as a volume in the
#   container's home directory
# - Should `--rm` container when done
# - Should use `-it` mode
```

### With `docker-compose`

### Use this to lauch the docker container. Make sure you're in the my-datascience-notebook directory

Build and run:

```bash
cd ./OneDrive/Desktop/my-datascience-notebook/my-datascience-notebook
docker-compose up
# - It should publish port 8888
# - It should mount the local directory as a volume in the container's
#   home directory
#   Make sure that the image is tagged to dylanbolt/my-datascience-notebook. Under build simply put "." so that it looks in the local directory.
```
