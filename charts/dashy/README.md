# Dashy Helm Chart

Dashy helps you organize your self-hosted services by making them accessible from a single place.

## Original Project

+ Website: https://dashy.to/
+ Doc: https://dashy.to/docs
+ Repo: https://github.com/Lissy93/dashy

## Prerequisites

- Kubernetes 1.16+
- Helm 3+

## Get Repo Info

```console
helm repo add selfhosted-helmcharts https://vyrtualsynthese.github.io/selfhosted-helmcharts/
helm repo update
```

_See [helm repo](https://helm.sh/docs/helm/helm_repo/) for command documentation._

## Install Chart

```console
# Helm
$ helm install [RELEASE_NAME] selfhosted-helmcharts/dashy
```

_See [configuration](#configuration) below._

_See [helm install](https://helm.sh/docs/helm/helm_install/) for command documentation._

## Uninstall Chart

```console
# Helm
$ helm uninstall [RELEASE_NAME]
```

This removes all the Kubernetes components associated with the chart and deletes the release.

_See [helm uninstall](https://helm.sh/docs/helm/helm_uninstall/) for command documentation._

## Upgrading Chart

```console
# Helm
$ helm upgrade [RELEASE_NAME] [CHART] --install
```

_See [helm upgrade](https://helm.sh/docs/helm/helm_upgrade/) for command documentation._

## Configuration

See [Customizing the Chart Before Installing](https://helm.sh/docs/intro/using_helm/#customizing-the-chart-before-installing). To see all configurable options with detailed comments, visit the chart's [values.yaml](values.yaml), or run these configuration commands:

```console
# Helm 2
$ helm inspect values self-hosted/dashy

# Helm 3
$ helm show values self-hosted/dashy
```

You may similarly use the above configuration commands on each chart [dependency](#dependencies) to see it's configurations.
