# Servarr

Manage Sonarr, Radarr, Jackett, and Transmission w/ OpenVPN via docker compose. Substitues values from `.env` file.

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