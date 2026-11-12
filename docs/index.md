# Tally

Tally is tiny web analytics you host yourself. One script under 2 kB, no cookies, and one SQLite file for all your data.

- **Small:** the tracking script is 1.8 kB gzipped and loads asynchronously.
- **Private:** no cookies, no fingerprinting, and IP addresses are never stored.
- **Simple:** one binary, one SQLite database, one dashboard.

## Quick start

1. [Install Tally](install.md) on any server with Docker, or download the binary.
2. Add the tracking script to your site:

    ```html
    <script defer src="https://stats.example.com/tally.js" data-site="example.com"></script>
    ```

3. Open `https://stats.example.com` and log in with the admin password you set during install.

Page views show up within a few seconds. To count clicks, sign-ups or purchases, see [Track events](events.md).
