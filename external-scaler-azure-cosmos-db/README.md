# external-scaler-azure-cosmos-db

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.1.0](https://img.shields.io/badge/AppVersion-0.1.0-informational?style=flat-square)

Event-based autoscaler for Azure Cosmos DB change feed consumer applications

**Homepage:** <https://github.com/kedacore/external-scaler-azure-cosmos-db>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Ahmed ElSayed | <ahmels@microsoft.com> |  |
| Jatin Sanghvi | <jasanghv@microsoft.com> |  |
| Tom Kerkhove | <tomkerkhove@microsoft.com> |  |

## Source Code

* <https://github.com/kedacore/external-scaler-azure-cosmos-db>

## Requirements

Kubernetes: `>=v1.17.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalLabels | object | `{}` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"ghcr.io/kedacore/external-scaler-azure-cosmos-db"` |  |
| image.tag | string | `"0.1.0"` |  |
| port | int | `4050` |  |
| resources.limits.cpu | string | `"100m"` |  |
| resources.limits.memory | string | `"512Mi"` |  |
| resources.requests.cpu | string | `"10m"` |  |
| resources.requests.memory | string | `"128Mi"` |  |

