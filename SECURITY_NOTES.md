# Security Review Before Publishing

This repository was prepared for public portfolio use. Evidence was selected with the goal of showing the technical work without publishing unnecessary secrets.

## Safe to Publish

The screenshots included in `assets/screenshots/` were selected because they do not expose the SafeLine administrator password, certificate private-key contents, or active PHP session-cookie values.

The screenshots do contain private RFC1918 addresses (`192.168.2.x`). These are local lab addresses and are not publicly routable. They are retained because they help explain the network flow and testing evidence.

## Intentionally Excluded

The following types of screenshots from the working session should not be uploaded publicly:

- SafeLine installation output containing the generated administrator password
- Certificate-import screens displaying private-key text
- Any screenshot where the local SafeLine test password is visible
- Detailed SQL-injection request views that expose `PHPSESSID` or other session-cookie values
- Temporary copies of the certificate private key

## Credentials

Public documentation should not include:

- SafeLine administrator credentials
- SafeLine test-user password
- MySQL/DVWA database password
- Private-key material
- Active session identifiers

Use placeholders if a future setup guide requires credentials.

## Final Publishing Check

Before pushing the repository to GitHub:

1. Confirm only the sanitized `assets/screenshots/` directory is uploaded.
2. Do not upload the original raw screenshot collection.
3. Do not upload `dvwa.key`, database configuration files containing passwords, browser profiles, VM files, or SafeLine configuration backups containing secrets.
4. Review the Git diff before the first push.
5. Keep the lab isolated from production networks and update Kali, Ubuntu, and SafeLine regularly.
