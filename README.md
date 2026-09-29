# Automated Cloud Deployment Pipeline (CI/CD)

Production-ready infrastructure template demonstrating automated continuous delivery to an Ubuntu VPS.

### Stack & Architecture
- **Cloud Provider:** DigitalOcean Droplet (Ubuntu 24.04 LTS)
- **Containerization:** Docker & Docker Compose
- **Web Server:** Nginx (Alpine)
- **CI/CD Automation:** GitHub Actions
- **Security:** Ed25519 SSH Key authentication & Encrypted Secrets

### Live Demo
- **Server IP:** `http://104.248.243.88`

### Workflow Overview
Every push to the `main` branch triggers an isolated GitHub Actions runner that connects to the host via encrypted SSH credentials, updates the build, and performs a zero-downtime container reload.
