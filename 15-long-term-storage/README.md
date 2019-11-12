# Long Term Storage

## Presenter only

```
kubectl apply -f https://raw.githubusercontent.com/m3db/m3db-operator/v0.2.0/bundle.yaml --namespace default
kubectl apply -f https://raw.githubusercontent.com/m3db/m3/master/kube/sysctl-daemonset.yaml --namespace default
```

## Everyone

Install etcd
```
kubectl apply -f https://raw.githubusercontent.com/m3db/m3db-operator/v0.2.0/example/etcd/etcd-basic.yaml
```

Install m3db
```
kubectl apply -f m3db.yaml
kubectl apply -f service-monitor.yaml
kubectl apply -f m3db-dashboard.yaml
kubectl apply -f datasource.yaml
```

Update prometheus
```
helm upgrade --install -f values-instance.yaml prom-<YOURNAME> stable/prometheus-operator
```
