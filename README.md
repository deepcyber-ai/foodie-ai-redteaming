# Foodie AI — Red Teaming

Black-box penetration testing samples and methodology for the Foodie AI API.

## Structure

- `humanbound/` — manual, human-driven attack scenarios

## Setup

Tests target a live API endpoint. Configure credentials via environment variables (never hardcode):

```bash
export FOODIE_API_URL="https://your-api-url.amazonaws.com/dev"
export FOODIE_API_KEY="your-api-key"
```
