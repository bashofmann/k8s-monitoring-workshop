## Monitoring Services

## Everyone

* Install quote-svc
```
helm upgrade --install quote-svc-<YOURNAME> helm-charts/quote-svc -f quote-svc-values.yaml
```

* Install hello-svc
```
helm upgrade --install hello-svc-<YOURNAME> helm-charts/hello-svc -f hello-svc-values.yaml
```

* Install web-application
```
helm upgrade --install web-application-<YOURNAME> helm-charts/web-application -f web-application-values.yaml
```
