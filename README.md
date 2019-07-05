# Consul (Slightly Modified) Image Build

The version of this hosted on [My Dockerhub](https://cloud.docker.com/repository/docker/amerenda/rpi-consul)

There are several pieces that are used to build this image:

* We start with an arm7 base image and add CA certificates in order to reach
  the HashiCorp releases server. These are useful to leave in the image so that
  the container can access Atlas features as well.
* Finally a specific Consul build is fetched and the rest of the Consul-specific
  configuration happens according to the Dockerfile.
