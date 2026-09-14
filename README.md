# PULSE

**Meaningful change and event detection.**

> What just changed?

PULSE explores how systems can distinguish meaningful state changes from normal activity and expose the events that deserve attention.

## Why it exists

Complex systems produce enormous amounts of activity. Not every event deserves investigation.

PULSE is the observation edge of the ecosystem: it turns raw signals into **contextual, machine-readable changes** that downstream systems can investigate or act on.

## What it does

- ingest system signals
- normalize events
- detect meaningful change
- correlate related activity
- attach context and confidence
- emit machine-readable change events

## Use cases

| Use case | Question answered |
| --- | --- |
| Change detection | What changed from the expected state? |
| Monitoring | Which activity is meaningful enough to surface? |
| Deployment analysis | What changed around a deployment? |
| Configuration tracking | Which state changes deserve investigation? |
| Incident triggering | What event should start deeper analysis? |

## Architecture

```text
SIGNALS + EVENTS + STATE
          │
          ▼
       NORMALIZE
          │
          ▼
      CHANGE DETECTION
          │
          ▼
       CORRELATION
          │
          ▼
     MEANINGFUL EVENT
          │
          ├──► TRACE
          ├──► BLACKBOX
          └──► WAKE
```

## Ecosystem

PULSE is the observation edge of the core TITO systems chain. `GRID` supplies topology context and `TIME-MACHINE` supplies historical state.

## Status

Early research and architecture.

- [Architecture](docs/architecture.md)
- [Roadmap](docs/roadmap.md)

## License

MIT.