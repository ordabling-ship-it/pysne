# pysne

A simple Python Flask web service.

## Features
- REST API endpoints
- Health check endpoint
- Runs on configurable port via PORT environment variable

## Deployment

Deploy the free Render Blueprint:

1. Sign in to Render and select **New +** → **Blueprint**.
2. Connect GitHub and select `ordabling-ship-it/pysne`.
3. Review the `pysne` service from `render.yaml` and select **Apply**.

The Blueprint creates a free web service and configures its build, production
server, port, and health check. No environment variables or secrets are needed.
Render's free service may spin down after inactivity. Once deployment finishes,
open the generated `onrender.com` URL; `/health` should return
`{"status":"healthy"}`.

## Endpoints
- `GET /` - Main endpoint
- `GET /health` - Health check
