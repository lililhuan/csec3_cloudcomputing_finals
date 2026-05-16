# FIXIT Deployment Report

## Deployed Resources (Render)
- Service: Render Web Service
- Service Name: habitflow-app
- Runtime: Docker (Python 3.11)
- Region: Singapore (southeastasia)
- Deployment Type: Web Service (Docker)

## Service Configuration
- Type: Render Web Service
- Runtime: Docker (uses project's Dockerfile, Python 3.11)
- Region: Singapore
- State: Active
- HTTPS: Enabled (auto-provisioned TLS)
- Public Network Access: Enabled

## Web App Endpoint
- Live URL: https://v2-habitflow-app.onrender.com

## Notes
- This deployment uses Render's Free tier for academic use. Free tier services may sleep after ~15 minutes of inactivity, causing a short cold-start delay on the first request.
- For always-on production use, consider upgrading to Render Starter (~$7/month ≈ ₱400/month).
