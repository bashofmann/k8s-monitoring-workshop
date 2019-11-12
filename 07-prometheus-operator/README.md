# Monitoring

## Only presenter

```
helm upgrade --install -f values-operator.yaml prometheus-operator stable/prometheus-operator --namespace prometheus-operator
```

## Everyone

Update domain names in values.yaml and install prometheus

```
kubectl apply -f basic-auth.yaml
helm upgrade --install -f values-instance.yaml prom-<YOURNAME> stable/prometheus-operator
```
