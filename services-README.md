# services

This repository defines and manages homelab services running in Docker or K3s.

## Contents

- `docker-compose.yml` files grouped by service (e.g., Ghost, Portainer, reverse proxy)
- `.env` files for secrets and configuration (never commit sensitive values)
- Optional Helm charts or K3s manifests (in `k8s/` directory if added)

## Goals

- Enable easy deployment and upgrades of services
- Standardize configuration across environments
- Serve as the runtime application layer of the homelab

## Getting Started

```bash
git clone git@github.com:<your-username>/homelab-services.git ~/code/homelab/services
cd ~/code/homelab/services
docker compose up -d
```
