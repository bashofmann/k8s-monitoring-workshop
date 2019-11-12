# Monitoring nginx-ingress-controller

## Everyone

```
kubectl apply -f blackbox-exporter-config.yaml
kubectl apply -f blackbox-exporter-deployment.yaml
kubectl apply -f service-monitor.yaml
kubectl apply -f dashboard.yaml
```
