# Security Policy

## Supported Versions

This is an early-stage prototype; only the latest commit on `master` is supported.

## Reporting a Vulnerability

Please report security issues through GitHub's **Private Vulnerability Reporting**:

1. Go to the **Security** tab of this repository
2. Click **"Report a vulnerability"**
3. Fill in the advisory form

Reports are read by the maintainer and triaged within 7 days.

Please do **not** open a public issue for security problems.

## Scope

This project is a static, browser-only HTML5/Canvas game prototype with **no
server, no backend, no user accounts, no third-party JavaScript dependencies**.
The realistic attack surface is limited to:

- DOM/XSS issues introduced into game UI
- Asset loading paths (images served from `/public/`)
- Hosting platform misconfiguration (GitHub Pages)

If you find anything in those areas, the report is welcome.
