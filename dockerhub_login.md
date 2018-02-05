### Oreta images on Dockerhub

>Docker Hub is a registry for creating  both public and private repositories and storing and sharing docker images.

### How to login to dockerhub?

> Note: You must use Docker Engine 1.6 or later to push to Docker Hub. Follow the official installation instructions to install docker [https://docs.docker.com/install/](https://docs.docker.com/install/)


```
# docker login
Login with your Docker ID to push and pull images from Docker Hub. 
If you don't have a Docker ID, head over to https://hub.docker.com 
to create one.

Username: oretahub
Password: < will be provided via email>

Login Succeeded
```

### How to push a docker image to dockerhub ?

1. Create a docker image
>  You can clone this repo 
> [https://github.com/OretaHub/cloudnative2.0](https://github.com/OretaHub/cloudnative2.0) to create a local docker image
> call the image hugocn

2. Create a tag for the local docker image with the dockerhub registry name. 
```docker tag hugocn oretahub/hugocn:v1.3 ```
3. push the image to the dockerhub registry

```
# docker push oretahub/hugocn:v1.3
The push refers to repository [docker.io/oretahub/hugocn]
c7031cb4189f: Pushed
68695a6cfd7d: Pushed
c1dc81a64903: Pushed
8460a579ab63: Pushed
d39d92664027: Pushed
v1.3: digest: sha256:5e1dcxxxxd1abxxxxxd0da02xxxxxc 
size: 1364
```

### How to pull a docker image from dockerhub?

```
# docker pull oretahub/hugocn:v1.3

v1.3: Pulling from oretahub/hugocn
Digest: sha256:5e1dcxxxxd1abxxxxxd0da02xxxxxc
Status: Image is up to date for oretahub/hugocn:v1.3
```



