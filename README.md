# Alpine Nginx

Tiny web server using nginx built from source on the latest Alpine Linux.

The current version of Nginx availble in apk is outdated, this image tries to cope with the latest version available for nginx.

This image builds the latest version (1.9.4) from source:

```sh
docker run -it --rm efrecon/docker-alpine-nginx sh

> nginx -v
nginx version: nginx/1.9.4
```

Built image currently weighs in at 29.28 MB:

```sh
❯ docker images | grep alpine-nginx
efrecon/docker-alpine-nginx                      latest              b80c683a1fed        25 minutes ago      29.28 MB
```
