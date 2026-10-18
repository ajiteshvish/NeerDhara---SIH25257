# Sensor data

## What a node measures

| Field | Unit | Purpose |
| --- | --- | --- |
| Tank level | percent | Early cleaning and overflow-risk detection |
| High-water float | yes/no | Independent high-level safety input |
| Flood wetness | yes/no | Unit and village flood mode |
| Flap position input | yes/no | Prototype mechanical-state input |
| Battery | volts | Low-power warning |
| Radio signal | dBm | Connectivity diagnosis |
| Turbidity | NTU | Optional community-unit water-quality input |
| Flow | litres/minute | Optional community-unit throughput input |

The firmware publishes a regular reading every five minutes and can publish sooner when a configured limit is
crossed. A node keeps an increasing sequence number so repeated deliveries are stored once.

## Message fields

A reading carries these compact fields:

| Field | Meaning |
| --- | --- |
| `seq` | Increasing reading number |
| `ts` | Reading time in UTC, or empty when the node clock is not ready |
| `level_pct` | Tank level from 0 to 120 percent |
| `float_tripped` | High-water float state |
| `flood_wet` | Flood sensor state |
| `flap_closed` | Prototype flap input state |
| `turbidity_ntu` | Optional turbidity reading |
| `flow_lpm` | Optional flow reading |
| `battery_v` | Battery voltage |
| `rssi` | Radio signal strength in dBm |

Messages can contain one reading or a small buffered batch. Invalid readings are rejected; a missing or implausible
node time is replaced by arrival time and marked accordingly.

