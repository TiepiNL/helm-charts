# capacitor

A Helm chart for deploying capacitor, a general purpose UI for FluxCD.

This chart is based on https://github.com/sebastiangaiser/helm-charts/tree/main/charts/capacitor.

## Network policies
Currently only Kubernetes native `NetworkPolicy` is supported.
Check the values how to configure the flavor.

## Parameters

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` | Affinities |
| capacitor.readonly | bool | `true` |  |
| capacitor.showEvents | bool | `true` |  |
| capacitor.showPodLogs | bool | `true` |  |
| capacitor.showSecrets | bool | `true` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/gimlet-io/capacitor"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress | object | `{"annotations":{},"className":"","enabled":false,"hosts":[{"host":"capacitor.example.com","paths":[{"path":"/","pathType":"ImplementationSpecific"}]}],"tls":[]}` | Ingress |
| livenessProbe | object | `{}` | Liveness probe |
| nameOverride | string | `""` |  |
| namespaceOverride | string | `""` |  |
| networkPolicy | object | `{"enabled":true,"flavor":"kubernetes"}` | Network Policy |
| networkPolicy.flavor | string | `"kubernetes"` | kubernetes |
| nodeSelector | object | `{}` | Node selectors |
| podAnnotations | object | `{}` |  |
| readinessProbe | object | `{"failureThreshold":3,"httpGet":{"path":"/","port":9000,"scheme":"HTTP"},"initialDelaySeconds":0,"periodSeconds":10,"successThreshold":1,"timeoutSeconds":3}` | Readiness probe |
| replicaCount | int | `1` |  |
| resources | object | `{"requests":{"cpu":"200m","memory":"200Mi"}}` | Resources |
| securityContext | object | `{}` | Security context |
| service | object | `{"annotations":{},"labels":{},"port":9000,"type":"ClusterIP"}` | Service |
| serviceAccount | object | `{"annotations":{},"create":true}` | ServiceAccount |
| tolerations | list | `[]` | Toleration's |
