# System Architecture

## Layers

### Android presentation
Kotlin and Jetpack Compose with Material 3. Screens, navigation, UI state and ViewModels follow an MVVM-oriented presentation approach.

### Domain
Business rules and computation engines support crop, farm, finance, water and market calculations. BhoomiAgentOrchestrator coordinates the market decision workflow.

### Data
Repositories abstract data access. Room/SQLite provides local persistence; cache and DataStore support offline-first and preference workflows.

### External integrations
- Firebase AI / Gemini for conversational and image-assisted AI workflows.
- Open-Meteo for weather information.
- Google Fused Location Provider for device location.
- Government mandi and provider feeds where configured and validated.

## Simplified data path

1. The farmer supplies a question, image, crop/quantity or farm context.
2. A ViewModel coordinates the relevant domain use case.
3. Domain logic validates inputs and applies calculations or orchestrates retrieval.
4. Repositories read/write local records and retrieve external data where connectivity is available.
5. The application presents guidance, comparisons, estimates and data-status indicators.

## Offline behaviour

Farm records and cached information can be available locally. Fresh remote AI, weather and market responses require connectivity. Offline operation should not be represented as live access to external services.

## Scheduling

Weather/advisory checks are scheduled work, not continuous background monitoring. Use the scheduling mechanism actually implemented in the current app build; do not document an assumed scheduler as implemented until verified.
