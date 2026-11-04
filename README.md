# CarePoint — Hospital Management System

A classic, responsive hospital-management interface for an academic/demo project. Built with HTML, CSS, and vanilla JavaScript.

## Features

- Hospital overview dashboard
- Patient registration and patient directory search
- Patient record detail view
- Doctor directory and appointment overview
- QR identity pass generation and printing
- QR scanning with camera or manual patient ID
- Browser-local demo records (`localStorage`)
- Responsive desktop and mobile layout

## Run locally

Open `index.html` in a browser, or serve the folder with a local web server:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Demo and privacy notice

**This is not a production medical system. Use fictional/sample data only.** The sample patients and any records entered are stored in the current browser's `localStorage`. This is not a secure database and there is no authentication or authorization. The QR contains only a CarePoint patient identifier; the record is resolved within this demo.

Before using real patient data, build a secured backend with authenticated staff accounts, server-side authorization, encrypted transport/storage, audit logs, consent/retention controls, and a compliant hosting environment. Do not publish real patient data to GitHub Pages.

## GitHub Pages

This repository includes a GitHub Actions workflow (`.github/workflows/pages.yml`) that deploys the static site to GitHub Pages when code is pushed to the `main` branch. In GitHub, set **Settings → Pages → Build and deployment → Source** to **GitHub Actions**. The first workflow run will publish the demo.

## Tech stack

- HTML5
- CSS3
- Vanilla JavaScript
- QRCode.js (QR generation)
- html5-qrcode (camera scanning)
