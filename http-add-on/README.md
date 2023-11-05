# keda-add-ons-http

![Version: 0.4.1](https://img.shields.io/badge/Version-0.4.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.4.0](https://img.shields.io/badge/AppVersion-0.4.0-informational?style=flat-square)

Event-based autoscaler for HTTP workloads on Kubernetes

**Homepage:** <https://github.com/kedacore/http-add-on>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Ahmed ElSayed | <ahmels@microsoft.com> |  |
| Jorge Turrado | <jorge_turrado@hotmail.es> |  |
| Tom Kerkhove | <kerkhove.tom@gmail.com> |  |
| Zbynek Roubalik | <zroubali@redhat.com> |  |

## Source Code

* <https://github.com/kedacore/http-add-on>

## Requirements

Kubernetes: `>=v1.23.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalLabels | string | `""` |  |
| crds.install | bool | `true` |  |
| images.interceptor | string | `"ghcr.io/kedacore/http-add-on-interceptor"` |  |
| images.kubeRbacProxy.name | string | `"gcr.io/kubebuilder/kube-rbac-proxy"` |  |
| images.kubeRbacProxy.tag | string | `"v0.13.0"` |  |
| images.operator | string | `"ghcr.io/kedacore/http-add-on-operator"` |  |
| images.scaler | string | `"ghcr.io/kedacore/http-add-on-scaler"` |  |
| images.tag | string | `nil` |  |
| interceptor.admin.port | int | `9090` |  |
| interceptor.admin.service | string | `"interceptor-admin"` |  |
| interceptor.affinity | object | `{}` |  |
| interceptor.deploymentCachePollingIntervalMS | int | `250` |  |
| interceptor.expectContinueTimeout | string | `"1s"` |  |
| interceptor.forceHTTP2 | bool | `false` |  |
| interceptor.idleConnTimeout | string | `"90s"` |  |
| interceptor.imagePullSecrets | list | `[]` |  |
| interceptor.keepAlive | string | `"1s"` |  |
| interceptor.maxIdleConns | int | `100` |  |
| interceptor.nodeSelector | object | `{}` |  |
| interceptor.proxy.port | int | `8080` |  |
| interceptor.proxy.service | string | `"interceptor-proxy"` |  |
| interceptor.pullPolicy | string | `"Always"` |  |
| interceptor.replicas.max | int | `50` |  |
| interceptor.replicas.min | int | `3` |  |
| interceptor.replicas.waitTimeout | string | `"20s"` |  |
| interceptor.resources.limits.cpu | float | `0.5` |  |
| interceptor.resources.limits.memory | string | `"64Mi"` |  |
| interceptor.resources.requests.cpu | string | `"250m"` |  |
| interceptor.resources.requests.memory | string | `"20Mi"` |  |
| interceptor.responseHeaderTimeout | string | `"500ms"` |  |
| interceptor.routingTableUpdateDurationMS | int | `500` |  |
| interceptor.scaledObject.pollingInterval | int | `1` |  |
| interceptor.tcpConnectTimeout | string | `"500ms"` |  |
| interceptor.tlsHandshakeTimeout | string | `"10s"` |  |
| interceptor.tolerations | list | `[]` |  |
| operator.adminPort | int | `9090` |  |
| operator.adminService | string | `"operator-admin"` |  |
| operator.affinity | object | `{}` |  |
| operator.imagePullSecrets | list | `[]` |  |
| operator.nodeSelector | object | `{}` |  |
| operator.port | int | `8443` |  |
| operator.pullPolicy | string | `"Always"` |  |
| operator.resources.limits.cpu | float | `0.5` |  |
| operator.resources.limits.memory | string | `"64Mi"` |  |
| operator.resources.requests.cpu | string | `"250m"` |  |
| operator.resources.requests.memory | string | `"20Mi"` |  |
| operator.tolerations | list | `[]` |  |
| operator.watchNamespace | string | `""` |  |
| scaler.affinity | object | `{}` |  |
| scaler.grpcPort | int | `9090` |  |
| scaler.healthPort | int | `9091` |  |
| scaler.imagePullSecrets | list | `[]` |  |
| scaler.nodeSelector | object | `{}` |  |
| scaler.pendingRequestsInterceptor | int | `200` |  |
| scaler.pullPolicy | string | `"Always"` |  |
| scaler.service | string | `"external-scaler"` |  |
| scaler.tolerations | list | `[]` |  |

