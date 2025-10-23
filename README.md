# gatus-controller
See https://github.com/TwiN/gatus/issues/393

> :warning: This is planned for the future. See https://github.com/home-operations/gatus-sidecar for a good Kubernetes native solution


Support annotations such as the following on Kubernetes services:
```yaml
gatus.io/config: |
  endpoints:
    - name: example
      url: https://example.org
      interval: 10m
      conditions:
        - "[STATUS] == 200"
```

### Limitations
- TODO: Prevent any configuration that is not under `endpoints[]` (e.g. no `alerting.slack` or `ui.title` config) 
