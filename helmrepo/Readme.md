This is Netdata's Traefik 2 Helm repository.

# Use

To use this repo with helm, add the repository:

```
helm repo add netdata-traefik https://netdata.github.io/traefik-helm-chart/helmrepo/
helm repo update
```

Install the traefik chart:

```
helm install traefik netdata-traefik/traefik
```

# Update helm package repo

```
helm package traefik-helm-chart-master-root/traefik
helm repo index .
```
