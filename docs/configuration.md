# Configuration

Tally is configured with environment variables.

| Variable | Default | What it does |
|---|---|---|
| `TALLY_ADMIN_PASSWORD` | none, required | Password for the dashboard |
| `TALLY_PORT` | `8080` | Port to listen on |
| `TALLY_DATA` | `/data` | Folder for the SQLite database and backups |
| `TALLY_RETENTION_DAYS` | `730` | Raw events older than this are deleted; daily totals are kept forever |
| `TALLY_IGNORE_BOTS` | `true` | Drop requests from known crawlers |
| `TALLY_PUBLIC` | `false` | Make the dashboard readable without logging in |

## Several sites

One Tally server can track any number of sites. Each site is created the first time a page view with a new `data-site` value arrives; there is nothing to set up in advance.

## Excluding your own visits

Open your site with `?tally=ignore` once. Tally sets a flag in local storage and stops counting visits from that browser. Use `?tally=count` to undo it.
