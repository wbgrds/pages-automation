# GitHub Pages Automation

Automatisierte Erstellung von GitHub Pages Sites mit Hetzner DNS.

## Setup

### 1. GitHub Token
Dein Token ist bereits konfiguriert.

### 2. Hetzner Token als Secret
- Repository → Settings → Secrets and variables → Actions
- New repository secret:
  - **Name:** `HETZNER_TOKEN`
  - **Value:** Dein Hetzner DNS API Token

### 3. Workflow ausführen
- Geh zu: Actions → "Deploy GitHub Pages + Hetzner DNS"
- Klick: "Run workflow"
- Gib ein:
  - Subdomain: `prototype`
  - Domain: `ob5.dev`
- Klick: "Run workflow"

## Fertig
Der Workflow erstellt:
1. Repo: `wbgrds/dev.ob5.prototype`
2. GitHub Pages aktiviert
3. Hetzner CNAME konfiguriert
4. Standard-Seite deployed

DNS propagiert in 5-10 Minuten.