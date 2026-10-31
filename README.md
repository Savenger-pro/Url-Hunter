# LinkLens

A browser-only phishing and malware link checker. No server, no install, no build step.

## What it shows

- A 0 to 100 risk score with a clear verdict
- Exactly which words, code snippets, forms or frames triggered each warning
- Domain details: registrar, registration date, domain age, expiry, name servers
- Hosting details: IP addresses, hosting provider, ASN, server location

## Run it online with GitHub Pages

1. Create a new GitHub repository and upload `index.html` and `README.md`.
2. Open **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. After a minute your tool is live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

## Data sources

| Purpose | Service |
| --- | --- |
| DNS records | Google Public DNS |
| Domain ownership | RDAP via rdap.org |
| IP and hosting | ipwho.is |
| Page source | AllOrigins proxy |

Browsers block direct cross-site page requests, so the page source is fetched through a public proxy. If it is unavailable, use the **Paste page source** tab.

## Limits

This is a rule-based checker. A low score does not prove a site is safe.
