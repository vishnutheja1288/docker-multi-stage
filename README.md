# docker-multi-stage
multistage docker file using distroless images

$ docker build -t vsihnutheja88/nodejs:v1 --no-cahe -f Dockerfile1 .

$ docker images

$ docker build -t vsihnutheja88/nodejs:v2 --no-cache -f Dockerfile2 .

$ docker images ls

check the both images size.
using the multistage we will reduce the size of docker image up to 80%
