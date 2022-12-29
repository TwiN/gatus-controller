# gatus-controller
See https://github.com/TwiN/gatus/issues/393


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
