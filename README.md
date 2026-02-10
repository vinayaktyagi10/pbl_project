# SDC Infrastructure Automation - PBL Semester 4

A high-resilience infrastructure presentation built with [Slidev](https://sli.dev/).

## Features
- **Modern Tech Stack:** Built with Vue, Vite, and Markdown.
- **Architectural Diagrams:** Powered by Mermaid.js.
- **Developer First:** Focuses on engineering principles (Zero Trust, cgroups, RPO/RTO).
- **Auto-Deploy:** Integrated GitHub Actions for seamless hosting on GitHub Pages.

## Getting Started

### Local Development
1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the dev server:
   ```bash
   npm run dev
   ```
3. Open `http://localhost:3030` in your browser.

### Key Commands
- `o`: Overview mode
- `p`: Presenter mode
- `m`: Toggle drawings

## Deployment
This project is configured to auto-deploy to GitHub Pages via GitHub Actions.
1. Push changes to the `main` branch.
2. Ensure **Settings > Pages > Build and deployment > Source** is set to **GitHub Actions**.

## Project Highlights
- **Resilient Backups:** Incremental snapshot logic using rsync hard-links.
- **Security:** Zero Trust Mesh VPN (Tailscale).
- **Stability:** Linux kernel-level resource constraints (cgroups).
- **Modern Storage:** Migration to S3-compatible Object Storage (MinIO).