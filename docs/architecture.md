# PULSE Architecture

PULSE turns raw system activity into meaningful change events.

## Flow

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
       ┌──┼──┐
       ▼  ▼  ▼
     TRACE BLACKBOX WAKE
```

## Design principles

1. Normal activity should not automatically become an incident.
2. Change detection retains source context.
3. Related events can be grouped without erasing individual evidence.
4. Meaning is contextual and should remain inspectable.
5. Output is machine-readable and suitable for downstream investigation.