# Node JS Server Docker


## Building a new image

In the directory where the Dockerfile is :

```sh
docker build -t bpi/nodejs_server .
```

## Testing locally

Port 3000 of the container must be mapped to the localhost 3000 port

```sh
docker run -p 3000:3000 bpi/nodejs_server
```

## Tagging an image

To version images, you can tag it with a x.y version and also assign the latest tag. The latest tag is the one pulled in Saagie.

```sh
docker tag bpi/nodejs_server bpi/nodejs_server:<x.y>
docker tag healbpithyhealth/nodejs_server bpi/nodejs_server:latest
```


## Pushing to Docker Hub repository

```sh
docker push bpi/nodejs_server
```
