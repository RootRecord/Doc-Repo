# Weather data pipeline (conceptual)

## Upstream

Providers (e.g. AccuWeather) and **NOAA** feeds supply raw meteorological and alert content.

## Worker middle layer

- **Crons** fetch upstream payloads on schedules.
- **TTL caches** avoid hammering paid APIs for identical grid points (`WEATHER_DATA_TTL_SEC`).

## Downstream

Mobile apps request **bundles** that combine current conditions, forecasts, and alert collections suitable for UI cards.

## Teaching users

“Refresh” in UI **does not** always bypass server caches—this saves money and keeps responses fast.

## Related reading

- [../02-products/weather-manager.md](../02-products/weather-manager.md)
