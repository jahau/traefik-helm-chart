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
git worktree add src master

helm package src/traefik
helm repo index .

git worktree remove src
```

replace `master` with appropriate commit-ish of the source repo.
