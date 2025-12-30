# Helm Charts

Custom Helm charts for [k8s-platform-core](https://github.com/TiepiNL/k8s-platform-core) platform components.

This repository provides Helm charts for Kubernetes resources that either lack official charts or require customized packaging for GitOps deployment patterns.

Charts are hosted via GitHub Pages at: `https://TiepiNL.github.io/helm-charts/`

## Usage

Tl;dr:

```bash
helm repo add tiepi https://TiepiNL.github.io/helm-charts/
helm repo update
helm search repo tiepi/
```
