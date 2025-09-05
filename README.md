# Office Nextcloud Deployment (office.upcube.ai)

This repo contains the Docker Compose setup for the **Office Nextcloud** instance with Collabora Online integration.

## Services
- **Nextcloud** (port 8090 → `office-nextcloud`)
- **MariaDB** (internal, `office-db`)
- **Collabora** (port 9982 → `office-collabora`)

## Requirements
- Docker 20+
- Docker Compose v2+

## Deployment

```bash
git clone https://github.com/upcubeinc/office.upcube.ai.git
cd office.upcube.ai

# Adjust environment values in `.env`
nano .env

# Start the stack
docker compose up -d
