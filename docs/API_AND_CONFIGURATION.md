# API and Configuration

## Integrations described by the project

| Service | Purpose | Validation requirement |
|---|---|---|
| Open-Meteo | Weather information | Verify requested location, units, timestamps and response |
| Firebase AI / Gemini | Conversational and image-assisted AI | Verify project configuration, model access and server/client key handling |
| Google Fused Location Provider | Device location | Verify permissions, location availability and fallback |
| Government mandi data feeds | Market prices | Verify API key, endpoint, schema, crop/market mapping and update time |
| Provider/warehouse information | Storage and provider discovery | Verify source, current availability, geography and contact details |

## Local configuration

Never commit API keys or credentials. Keep local values in ignored development configuration or a secure server-side secret store. Commit only a safe example file with placeholder values and explain how developers obtain their own credentials.

## Market-data validation checklist

- Endpoint responds successfully.
- Authentication is accepted.
- Requested filters return the expected crop, market and date.
- Price fields and units are interpreted correctly.
- Observation timestamp and source are retained.
- Missing, empty, malformed and rate-limited responses are handled.
- Cached data is visibly distinguished from newly retrieved data.

This document describes integration boundaries and validation steps; it does not assert that every external feed is currently live.
