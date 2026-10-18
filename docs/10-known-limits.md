# Known limits and next steps

Neerdhara is a working prototype, not a finished public infrastructure product.

## Current limits

- No live river-level, rainfall or weather forecast feed.
- No village population or ward dataset.
- No operator GPS tracking or arrival-time estimate.
- No app-sync failure telemetry or broker socket count.
- Voice calls are simulated; there are no delivery receipts, acknowledgements or retry reports.
- Firmware releases record SHA-256, but device-side remote update apply and signature verification are not complete.
- Device MAC address and hardware type are not stored.
- Treatment-stage debris and sludge are operator observations, not separate sensors.
- Household treated/reused quantities can be **estimated** rather than meter readings.
- Changing the hosted media store does not automatically move older files.

## What comes next

1. Calibrate sensors and treatment assumptions through a monitored village pilot.
2. Add consented messaging and voice delivery with status callbacks.
3. Integrate trusted rainfall and river feeds where available.
4. Complete signed device updates and field recovery procedures.
5. Define retention, support, maintenance and accessibility processes with implementing agencies.

