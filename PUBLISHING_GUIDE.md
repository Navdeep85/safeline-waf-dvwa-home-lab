# Publishing Guide - GitHub and LinkedIn

This package is designed so the lab computer does **not** need to be signed in to GitHub or LinkedIn. Copy/download the finished project on the other laptop and publish it from there.

## Recommended GitHub Repository

**Repository name:** `safeline-waf-dvwa-home-lab`

**Repository title / README title:** SafeLine WAF Home Lab with DVWA and Kali Linux

**Short description:**

> Home lab using SafeLine WAF, DVWA, Kali Linux, and Ubuntu Server to test HTTPS reverse proxying, SQL injection blocking, HTTP rate limiting, authentication, and source-IP deny rules.

**Suggested topics:**

`cybersecurity` `homelab` `waf` `safeline` `dvwa` `kali-linux` `ubuntu` `web-security` `sql-injection` `reverse-proxy`

## What to Upload

Upload the contents of this folder as the repository root:

- `README.md`
- `SECURITY_NOTES.md`
- `PUBLISHING_GUIDE.md`
- `.gitignore`
- `assets/screenshots/`
- `docs/SafeLine-WAF-Home-Lab-Report.pdf`
- `docs/SafeLine-WAF-Home-Lab-Report.docx` (optional; PDF is enough for most visitors)

Do **not** upload the original raw screenshot collection, VM files, private keys, passwords, browser data, or configuration backups containing secrets.

## GitHub Upload from the Other Laptop

The easiest approach is the GitHub website:

1. Sign in to GitHub on the other laptop.
2. Create a new public repository named `safeline-waf-dvwa-home-lab`.
3. Do not auto-create a README if you are uploading this finished package.
4. Choose **Add file -> Upload files**.
5. Upload the project contents while preserving the `assets/` and `docs/` folders.
6. Review the file list before committing.
7. Open the repository after upload and confirm all screenshots render inside the README.
8. Open the PDF report from GitHub and confirm it displays correctly.

## Final Security Check Before Publish

- No SafeLine admin password
- No SafeLine test-user password
- No MySQL/DVWA database password
- No certificate private-key content
- No `PHPSESSID` or browser/session-cookie values
- No VM disk images
- No raw screenshots outside the sanitized screenshot folder

## LinkedIn Project Entry

After the GitHub repository is live, add it to the **Projects** section of LinkedIn.

**Project name:** SafeLine WAF Home Lab with DVWA and Kali Linux

**Description:**

> Built a cybersecurity home lab using Kali Linux, Ubuntu Server, DVWA, and SafeLine WAF. Configured SafeLine as an HTTPS reverse proxy and validated SQL injection blocking, HTTP rate limiting, WAF authentication, and source-IP deny rules. Verified the controls using both client-side results and SafeLine security logs, and documented the troubleshooting and evidence in GitHub.

Add the GitHub repository URL as the project link.

## LinkedIn Post Draft

> I recently completed a Web Application Firewall home lab using Kali Linux, Ubuntu Server, DVWA, and SafeLine WAF.
>
> I configured SafeLine as an HTTPS reverse proxy in front of DVWA and tested several security controls from Kali, including SQL injection blocking, HTTP rate limiting, authentication, and a custom source-IP deny rule. I also verified the results in SafeLine logs instead of relying only on what the browser displayed.
>
> The troubleshooting was an important part of the project. I worked through VM networking, local hostname resolution, the DVWA application path, a MySQL compatibility issue, and SafeLine/Docker service checks.
>
> I documented the setup, test evidence, and lessons learned in GitHub: **[ADD GITHUB LINK]**
>
> #Cybersecurity #HomeLab #WebSecurity #WAF #KaliLinux #DVWA #Ubuntu #LearningByDoing

## Interview-Friendly 30-Second Explanation

> I built a small WAF lab with Kali as the testing machine and DVWA running on Ubuntu. SafeLine sat in front of DVWA as an HTTPS reverse proxy. I tested SQL injection, rate limiting, authentication, and an IP deny rule, then verified the results in SafeLine logs. The project also gave me troubleshooting practice with bridged networking, local name resolution, Apache paths, MySQL compatibility, and Docker service health.
