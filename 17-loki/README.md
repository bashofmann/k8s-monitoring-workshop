# Logging with Loki

## Everyone

```
helm repo add loki https://grafana.github.io/loki/charts
helm repo update
helm upgrade --install loki-<YOURNAME> loki/loki-stack -f loki-values.yaml
kubectl apply -f datasource.yaml
```
