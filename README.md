# Cyber Security Pilot website

Marketing site for Cyber Security Pilot: a practical cyber security roadmap
covering an external domain baseline (DNS, website, SPF/DKIM/DMARC monitoring),
an internal and process baseline (CIS v8 device audits) and vulnerability
scanning through NMapUI.

Live site (GitHub Pages): https://techmore.github.io/csp-www/

## Run or deploy

There is no build step. `index.html` is a single static page that loads
Tailwind (Play CDN), Lucide icons and Google Fonts at runtime.

- Preview locally: open `index.html` in a browser, or run
  `python3 -m http.server` in the repo root and visit http://localhost:8000.
- Deploy: push to `main`; GitHub Pages serves the repo root. (The `CNAME`
  file was removed, so the site is on the `github.io` address.)

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | The landing page: services, approach, vulnerability scanning, contact |
| `Chrome_Moysle_googleadmin/school-mac-security-roadmap.html` | School Mac security implementation checklist, linked from the landing page |
| `Chrome_Moysle_googleadmin/school-mac-chrome-goguardian-setup-guide.md` | Setup guide for school Macs managed with Mosyle, Google Admin (Chrome) and GoGuardian |
| `preview.png`, `preview-mobile.png` | Desktop and mobile screenshots of the landing page |

The landing page links out to the related sites
[TM-NMapUI-www](https://techmore.github.io/TM-NMapUI-www/) and
[tm-external-baseline](https://techmore.github.io/tm-external-baseline/).

## Status

Live. Content-only site with no tests or CI.
