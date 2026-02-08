# Foodie AI — Red Teaming

Black-box penetration testing samples and methodology for the Foodie AI API, aligned with the [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/).

## Structure

- `humanbound/` — adversarial security testing using [AIandMe](https://github.com/aiandme-io/aiandme-cli) (HumanBound)

## Quick start

```bash
cd humanbound
pip install -r requirements.txt
cp .env.example .env        # fill in your API credentials
aiandme login               # authenticate with AIandMe
python redteam.py full      # run the complete red teaming workflow
```

See [`humanbound/README.md`](humanbound/README.md) for full documentation.

## What's tested

| Category | Attack types |
|----------|-------------|
| Single-turn OWASP | Prompt injection, jailbreaks, data exfiltration |
| Multi-turn OWASP | Context manipulation, gradual escalation, conversational jailbreaks |
| Agentic | Goal hijacking, tool misuse, privilege escalation |
| Behavioral | Intent boundary validation, response quality |

## Credentials

All API credentials are loaded from `.env` files (gitignored). Never commit keys to this repo.
