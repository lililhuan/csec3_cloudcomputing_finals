# FIXIT Cost Estimate Report

## Architecture Summary
- Deployment platform: Render (Web Service)
- Database: SQLite (ephemeral or persistent depending on plan)

## Itemized Monthly Cost Breakdown (Render)
| Resource | Plan / Notes | Estimated Monthly Cost (PHP) |
|---|---|---:|
| Render Web Service | Free tier | ₱0 |
| SQLite on Persistent Disk | Included on Render plans where available | ₱0 |
| HTTPS / TLS | Included (auto-provisioned) | ₱0 |
| **Total (Free tier)** |  | **₱0 / month** |

### Notes
- The Render Free tier is used for this academic deployment. It is free (₱0/month) but has limitations: services spin down after ~15 minutes of inactivity, causing a short delay on the first request after idle.
- For a production setup, upgrade to Render Starter (~$7/month ≈ ₱400/month) to keep the service always running and avoid cold starts.

## Alternative: Azure (reference)
If your instructor prefers an Azure-based estimate, prepare an equivalent estimate using the Azure Pricing Calculator (App Service Free tier + Azure SQL Basic). Example (sample reference):

| Resource | Configuration | Estimated Monthly Cost (USD) |
|---|---|---:|
| App Service Plan (Basic) | B1, 1 instance (730 hours) | 13.14 |
| Resource Group | No direct charge | 0.00 |
| Web App | Billed through App Service Plan | 0.00 |
| **Estimated Total (sample)** |  | **13.14 USD** |

Estimated annual cost (sample): **157.68 USD**

![Azure Pricing Calculator Estimate](pricing-calculator-screenshot.png)

## Cost Optimization Notes
- Use free-tier or serverless offerings while developing and testing to minimize cost.
- Only upgrade to paid tiers (e.g., Render Starter or Azure Basic) when the app has active users and steady traffic.
- For production scaling, use reserved instances, autoscaling rules, and right-sized instance types to reduce costs.

## Recommendation
For this academic project, continue using Render's Free tier (₱0/month). If a smooth, always-on experience is required, upgrade to Render Starter (~₱400/month).

## References
- Render pricing and plans: https://render.com/pricing
- Azure Pricing Calculator: https://azure.microsoft.com/pricing/calculator/
