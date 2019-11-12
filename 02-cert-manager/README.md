# 7. cert-manager

## Presenter only

* Install and configure cert-manager for digital ocean
```
kubectl apply --validate=false -f https://raw.githubusercontent.com/jetstack/cert-manager/release-0.11/deploy/manifests/00-crds.yaml
helm repo add jetstack https://charts.jetstack.io
helm repo update
helm upgrade --install --namespace cert-manager --version v0.11.0 cert-manager jetstack/cert-manager
```

* Add Digital Ocean API Token to `digitalocean/digitalocean-dns-secret.yaml`

* Create ClusterIssuer
```
kubectl apply -f digitalocean/dns-secret.yaml
kubectl apply -f digitalocean/clusterissuer.yaml
```

* Create wildcard certificate
```
kubectl apply -f digitalocean/certificate.yaml
```
