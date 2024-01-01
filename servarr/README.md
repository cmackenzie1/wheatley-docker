# Servarr

Manage Sonarr, Radarr, Jackett, and Transmission w/ OpenVPN via docker compose. Substitues values from `.env` file.

## Installing Docker Manually on SynologyNAS

```bash
# Pick version from https://download.docker.com/linux/static/stable/x86_64/
wget https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz
tar xzvf docker-24.0.7.tgz
sudo cp docker/* /usr/local/bin
sudo dockerd &
sudo docker version
```

## `.env` file
| name | value | note |
|---|---|---|
|OPENVPN_PROVIDER | NORDVPN |
|OPENVPN_USERNAME | colemackenzie1@gmail.com |
|OPENVPN_PASSWORD | REDACTED |
|PUID | 1032 |
|PGID | 100 |
|TZ | America/Los_Angeles |

## Update all images to latest

```bash
docker-compose pull
```

## Template docker-compose.yml

```bash
docker-compose config
```

## Deploy

```bash
docker-compose up -d
```

## Destroy

```bash
docker-compose down
```
