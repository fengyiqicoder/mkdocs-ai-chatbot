# Install

Tally needs 64 MB of RAM and runs on Linux, macOS and Windows. A $5 VPS handles about 10 million page views a month.

## With Docker

```sh
docker run -d --name tally -p 8080:8080 \
  -v tally-data:/data \
  -e TALLY_ADMIN_PASSWORD=change-me \
  ghcr.io/example/tally:2
```

Put Tally behind a reverse proxy (Caddy, nginx) that handles HTTPS.

## As a binary

Download the latest release for your platform, then run:

```sh
TALLY_ADMIN_PASSWORD=change-me ./tally serve --port 8080 --data ./data
```

## Upgrading

Stop Tally, replace the image or binary, start it again. Database migrations run on start-up, and a backup of the database is written to `data/backups/` first.
