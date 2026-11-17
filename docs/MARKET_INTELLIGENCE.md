# Bhoomi Market Intelligence

## Purpose

Help a farmer compare selling choices based on more than a single mandi quote. The result is decision support; the farmer remains responsible for the final decision.

## Seven modules

1. **Dashboard** — harvest and market overview.
2. **My Harvest** — crop, variety, quantity and harvest records.
3. **Mandi Rates** — available minimum, maximum and modal price observations, with units and freshness labels.
4. **Nearby Mandis** — location-aware mandi discovery and distance comparison.
5. **Net Income Calculator** — estimated gross value less relevant costs such as transport, loading and mandi fees.
6. **AI Forecast & Sell-or-Wait** — trend analysis and forecast ranges when enough historical observations are available.
7. **Storage & Multi-Agent Coordination** — storage scenarios/ROI and consent-based provider enquiry workflows.

## Net-income reasoning

A basic estimate can be expressed as:

`Estimated net return = estimated gross sale value - estimated selling costs`

Clearly show which costs are entered by the farmer, retrieved from a verified source, estimated, or unavailable. Do not imply that an estimate is a guaranteed realised return.

## Forecast safeguards

Forecasts must be labelled as estimates and include uncertainty. When the required quantity or quality of historical observations is not available, suppress the forecast or explain why it cannot be generated. Do not invent confidence or accuracy values.

## Freshness and source status

Use clear states such as LIVE, CACHED, STALE, SAMPLE_DEMO and UNAVAILABLE where applicable. A configured endpoint is not proof of a working live feed. Validate the API key, endpoint, response schema, crop/market mapping, units and observation timestamp.

## Consent

Provider enquiries and any external coordination require explicit farmer approval. Recommendations do not trigger autonomous produce sales.
