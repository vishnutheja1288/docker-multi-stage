# docker-multi-stage
multistage docker file using distroless images

$ docker build -t vsihnutheja88/nodejs:v1 --no-cahe -f Dockerfile1 .

$ docker images

$ docker build -t vsihnutheja88/nodejs:v2 --no-cache -f Dockerfile2 .

$ docker images ls

check the both images size.
using the multistage we will reduce the size of docker image up to 80%

Method 2:
Using Distroless build images

$docker build -t vsihnutheja88/nodejs:v3 --no-cache -f Dockerfile3 .


Method 3:
Minimize the number of the layers in Dockerfile

$docker build -t vsihnutheja88/nodejs:v4 --no-cache -f Dockerfile4 .


Method 4:
Creation of docker images using Dockerfile4  and Dockerfile5, the Dockerfile5 docker image build time reduced compare with Dockerfile4.

Method 5: Cache usage
use the cache functionality better with Dockerfile6 than Dockerfile7 due to the better placement of the COPY command.

**Docker image optimization tools:**

  **Dive**: It is an image explorer tool that helps you discover layers in the Docker & OCI containers images
  
  **Docker Slim**: It helps you optimize your Docker images for security and size. you can reduce the docker image size upto 30x using slim
  
  **Docker Squash**: This utility helps you to reduce the image size by squashing image layers. The squash feature is also available in the Docker CLI using squash flag.
