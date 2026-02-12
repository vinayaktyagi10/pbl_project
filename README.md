# SDC Infrastructure Automation - PBL Semester 4

A high-resilience infrastructure portfolio and presentation built for Project Based Learning (PBL).

**Under the guidance of Dr. Dibakar Sinha**

## Features
- **Modern Tech Stack:** Built with Vue 3, Tailwind CSS, and Slidev.
- **Interactive Portfolio:** A professional landing page with custom UI/UX enhancements.
- **Themed Visuals:** Dracula-inspired design with custom-themed Mermaid.js diagrams.
- **Architectural Diagrams:** Visualized system flows and GitOps pipelines.
- **Developer First:** Focuses on engineering principles (Zero Trust, cgroups, RPO/RTO).
- **Auto-Deploy:** Integrated GitHub Actions for seamless hosting on GitHub Pages.

## Portfolio Enhancements
- **Scroll Progress Indicator:** Visual tracking of content reading.
- **Live System Status:** Operational heart-beat indicator in the navigation.
- **Code Snippet Utility:** One-click copy buttons for all technical snippets.
- **Observability View:** Static dashboard view of container health via Dozzle.

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