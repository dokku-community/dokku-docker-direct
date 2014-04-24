# dokku-docker-direct

Issue Docker commands via dokku.

## Installation

```bash
cd /var/lib/dokku/plugins
sudo git clone git@github.com:heichblatt/dokku-docker-direct.git docker-direct
sudo dokku plugins-install
```

## Issue Docker

Issue Docker command
```bash
docker-direct <app>
dodi <app>
```