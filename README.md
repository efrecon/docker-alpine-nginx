# Alpine Nginx

Tiny web server using nginx built from source on the latest Alpine Linux.

The current version of Nginx availble in apk is outdated, this image tries to cope with the latest version available for nginx. At presentm, this image builds the latest version (1.9.4) from source:

    docker run -it --rm efrecon/docker-alpine-nginx sh

    > nginx -v
    nginx version: nginx/1.9.4

Built image currently weighs in at 29.28 MB:

    ❯ docker images | grep alpine-nginx
    efrecon/docker-alpine-nginx                      latest              b80c683a1fed        25 minutes ago      29.28 MB

## Future Improvements

Cope with the more complex build command that is usually used for other [Linux distributions](http://nginx.org/en/linux_packages.html#mainline). This would provide a more capable web server, but should pay attention to resolving the necessary dependencies on Alpine.
