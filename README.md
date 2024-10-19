# helm-charts

This Helm chart repository has been created according to the steps described in [Turning your Github repository into a helm chart repository](https://purushothamkdr453.medium.com/turning-your-github-repository-into-a-helm-chart-repository-0bebd866eee0).

## Usage

Tl;dr:

```
helm repo add tiepinl https://tiepinl.github.io/helm-charts/

helm search repo tiepinl
```

## Roadmap

Create a Github Actions workflow to trigger  `helm package charts/capacitor/` and `helm repo index .` (update index.yaml) on a change of `Charts.yaml`.
