# Project Overview

## PRAKRUTI VIKAAS

PRAKRUTI VIKAAS is an Android agricultural intelligence companion developed and designed by Adithya Vishnubhatla. It connects farm-level records and guidance with market decision support.

## Context

The central hackathon challenge is that farmers can sell at the wrong time, place or price. A quoted mandi price alone does not account for distance, transport, handling, fees, storage, perishability or uncertainty.

## Product objectives

- Bring key agricultural workflows into one mobile application.
- Make farm context available to guidance and decision-support features.
- Compare market options using available price information and estimated costs.
- Clearly communicate data freshness and forecast uncertainty.
- Preserve farmer control over external enquiries and decisions.
- Support locally stored records when connectivity is limited.

## User-facing areas

1. Weather and location intelligence.
2. Bhoomi AI conversational support.
3. Plant Scanner and Crop Doctor.
4. Farms, plots, soil and growing conditions.
5. Seeds, inputs, germination and compost.
6. Irrigation, water ledger and harvest calendar.
7. Digital farm journal and farm expenses.
8. Bhoomi Market Intelligence.

## Current scope and evidence

The technical architecture report supplied for this project records Android v2.2.1 (Build 5), 22 destinations, 6 languages, 38 Room entities/tables, 20 DAOs, 27 computation engines and 70/70 automated tests passing. These are report-recorded metrics and should be checked against the current code and CI run.

Configured market-feed integrations require live endpoint validation before claiming that current market prices are operational.
