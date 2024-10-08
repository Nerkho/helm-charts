# core-keeper-dedicated

A Helm chart to deploy a Core Keep dedicated server

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

## Installing the Chart

```bash
helm repo add nerkho https://charts.nerkho.ch
helm repo update
helm install nerkho/core-keeper-dedicated core-keeper-dedicated -f values.yaml
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| config.dataPath | string | `""` |  |
| config.discord | string | `"0"` |  |
| config.discordHook | string | `""` |  |
| config.gameID | string | `""` |  |
| config.maxPlayers | string | `"10"` |  |
| config.season | string | `"-1"` |  |
| config.serverIP | string | `""` |  |
| config.serverPort | string | `""` |  |
| config.worldIndex | string | `"0"` |  |
| config.worldMode | string | `"0"` |  |
| config.worldName | string | `"Core Keeper Server"` |  |
| config.worldSeed | string | `"0"` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"escaping/core-keeper-dedicated"` |  |
| image.tag | string | `"latest"` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| volumes.serverData.mountPath | string | `"/home/steam/core-keeper-data"` |  |
| volumes.serverData.size | string | `"10Gi"` |  |
| volumes.serverData.storageClass | string | `nil` |  |
| volumes.serverFiles.mountPath | string | `"/home/steam/core-keeper-dedicated"` |  |
| volumes.serverFiles.size | string | `"10Gi"` |  |
| volumes.serverFiles.storageClass | string | `nil` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.13.1](https://github.com/norwoodj/helm-docs/releases/v1.13.1)
