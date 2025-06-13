# OTEL to Grafana Demo Stack

```mermaid
flowchart TB
    fluentbit[fluent-bit] -->|forwards| otel[OTEL Collector]
    otel --> Loki
    otel --> Prometheus
    otel --> Tempo
    Loki --> Grafana
    Prometheus --> Grafana
    Tempo --> Grafana
```

Sandbox for testing Fluent-bit to OTEL to LGTM stack forwarding.
