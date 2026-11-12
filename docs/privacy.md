# Privacy

Tally does not use cookies and does not store personal data, so in most cases you do not need a cookie banner for it. Check with your own legal advice if you are unsure.

## What is stored

For each page view: the page path, the referrer's domain, the browser and operating system family, the country (looked up from the IP address, which is then thrown away), and the screen size class (phone, tablet or desktop).

## How unique visitors are counted

Tally hashes the IP address and user agent together with a secret salt that changes every 24 hours. The hash lets Tally count a visitor once per day; after the salt changes, nobody, including you, can link a visit to an earlier one.

## Do Not Track

Tally respects the Do Not Track and Global Privacy Control signals by default. Set `TALLY_RESPECT_DNT=false` to count those visitors anyway.
