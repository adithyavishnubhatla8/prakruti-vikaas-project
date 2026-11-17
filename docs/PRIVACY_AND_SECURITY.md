# Privacy and Security

## Repository hygiene

Do not commit:
- API keys, passwords, access tokens or private certificates.
- Android signing keystores or signing credentials.
- local.properties or developer-specific machine configuration.
- Real farmer personal data, precise private farm records or private images.
- Production database exports or unredacted logs.

## Application principles

- Request only permissions needed for a feature.
- Explain location and camera use in context.
- Prefer local storage for farm records where appropriate.
- Use secure transport for network requests.
- Keep provider enquiries behind an explicit farmer-consent step.
- Distinguish observed facts, cached responses, estimates and predictions.
- Avoid presenting uncertain AI outputs as confirmed agronomic diagnoses.

## Reporting

Do not publish secrets or personal information in issues. Report suspected vulnerabilities privately to the repository owner.
