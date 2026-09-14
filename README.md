# PULSE

**Meaningful change and event detection.**

> What just changed?

PULSE explores how systems can distinguish meaningful state changes from normal activity and expose the events that deserve attention.

## What it does

- ingest system signals
- normalize events
- detect meaningful change
- correlate related activity
- attach context and confidence
- emit machine-readable change events

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