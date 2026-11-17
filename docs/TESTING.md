# Testing

## Reported test status

The supplied PRAKRUTI VIKAAS v2.2.1 technical architecture report records 70/70 automated tests passing across core, market and integration areas. Treat this as a report-recorded result, not as a current CI guarantee. Re-run the tests from the current source and attach the build/CI evidence before presenting it as current.

## Suggested test areas

- Room database creation, migrations and DAO behaviour.
- Offline reads/writes and cache freshness indicators.
- Location permission denial and manual-location fallback.
- Weather response parsing and unavailable states.
- Plant Scanner image suitability and failure handling.
- Crop guidance uncertainty and error handling.
- Mandi price parsing, units, timestamps and source status.
- Distance calculation and nearby-market ordering.
- Net-income calculation, missing cost inputs and edge cases.
- Forecast suppression when history is insufficient.
- Storage scenario assumptions and ROI calculations.
- Farmer-consent gate before provider enquiries.
- Regional-language UI and accessibility.
- End-to-end farmer scenario from crop/quantity input to recommendation.

## Reporting test results

Record the command, build variant, device/emulator, date, test count, passed/failed/skipped count and CI run URL. Do not claim coverage or accuracy unless measured.
