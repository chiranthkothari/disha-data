# disha-data

Compiled offline transit data bundles for **Disha**, a Delhi commuting app
(DTC buses + DMRC metro). This repository holds only build artifacts —
it is updated automatically by the app's data pipeline.

| File | Purpose |
|---|---|
| `manifest.json` | Current bundle version, size and SHA-256 |
| `delhi-transit.db` | The SQLite data bundle (stable URL, always latest) |

The app checks `manifest.json` and downloads `delhi-transit.db` when a
newer version is available.

## Data sources & attribution

- Bus data: Open Transit Data (Department of Transport, GNCTD) and the
  Transport Stack static GTFS.
- Metro station data via delhimetrorail.com.

Disha is not affiliated with DMRC or DTC.
