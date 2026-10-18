# Tech stack

| Technology | Why it fits |
| --- | --- |
| ESP32 | Low-cost controller with Wi-Fi, enough GPIO and broad local availability |
| MQTT | Lightweight, reconnect-friendly telemetry for constrained sensor nodes |
| FastAPI | Typed Python service with clear validation and asynchronous integrations |
| PostgreSQL | Reliable relational workflows for users, alerts, tasks and reporting |
| PostGIS | Spatial village boundaries, unit locations and flood-zone queries |
| Flutter | One accessible Android codebase for household, operator and panchayat roles |
| Next.js | Responsive official dashboard with server-assisted routing and localisation |
| React Query | Cached dashboard reads, polling and predictable refresh states |
| Drift | Structured local cache and durable offline action queue in the Android app |
| OpenStreetMap + Leaflet | Familiar, open map display for villages, units and flood layers |
| Recharts | Clear operational trends and report previews |

Hosted deployment uses a web host, container service, cloud database, MQTT broker and private media storage. Vendor
choices can change without changing the public workflow architecture.

