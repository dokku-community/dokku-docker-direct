# dokku-docker-direct [![Build Status](https://img.shields.io/travis/heichblatt/dokku-docker-direct.svg?branch=master "Build Status")](https://travis-ci.org/heichblatt/dokku-docker-direct)

Issue docker commands directly via a dokku plugin.

## requirements

- dokku 0.4.0+
- docker 1.8.x

## installation

```shell
# on 0.3.x
cd /var/lib/dokku/plugins
git clone https://github.com/heichblatt/dokku-docker-direct.git docker-direct
dokku plugins-install

# on 0.4.x
dokku plugin:install https://github.com/heichblatt/dokku-docker-direct.git docker-direct
```

## commands

```shell
docker-direct <command>        Issue docker command <command>
```

## usage

```shell
# view currently running containers
ssh dokku@your_host docker-direct ps

# list all images
ssh dokku@your_host docker-direct images

# inspect a container
ssh dokku@your_host docker-direct inspect $CID
```
