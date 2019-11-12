# Monitoring nginx-ingress-controller

## Presenter only

* Install nginx ingress controller:
```
kubectl label namespace nginx-ingress workshop-group=nginx-ingress
helm upgrade --install -f values.yaml --namespace nginx-ingress nginx-ingress stable/nginx-ingress
```

## Everyone

```
kubectl apply -f dashboard.yaml
```
