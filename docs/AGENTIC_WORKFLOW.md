# Agentic Workflow

## Goal

Coordinate the steps needed to compare selling options and explain trade-offs, while leaving all decisions with the farmer.

## Workflow

1. Collect crop, variety, quantity, location, harvest/readiness and relevant constraints.
2. Validate required inputs and identify missing data.
3. Retrieve available mandi observations and their timestamps/status.
4. Discover relevant nearby markets and calculate distance where coordinates are available.
5. Compare quoted prices and calculate estimated net return using available costs.
6. Analyse historical observations only when sufficient relevant data exists.
7. Evaluate storage alternatives, spoilage risk and cost assumptions where data is available.
8. Present ranked options with reasons, assumptions, missing information and uncertainty.
9. Ask the farmer before initiating any provider enquiry.
10. Record the farmer's chosen action where the app supports it.

## Human control

The orchestrator supports planning and recommendation. It does not make a sale, accept an offer or contact an external provider without explicit user consent.

## Failure handling

- No valid market response: show unavailable status; do not fabricate a price.
- Stale cached response: label it stale and show its timestamp if available.
- Insufficient history: do not generate an unsupported forecast.
- Missing cost inputs: show the estimate as incomplete and explain excluded costs.
- Provider details not verified: label them unverified and do not imply confirmed availability.
