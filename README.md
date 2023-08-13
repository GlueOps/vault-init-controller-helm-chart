# vault init controller

![Version: 0.1.0](https://img.shields.io/badge/Version-0.3.0-informational?style=flat-square)

A Helm chart to deploy vault init controller in kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| appEnv | string | `"dev"` | Environment of the application |
| appName | string | `"example-app"` | Name of the application |
| appVersion | string | `"0.0.1"` | Version of the application |
| commonAnnotations | string | `nil` | Common annotations for all Kubernetes objects |
| commonLabels | string | `nil` | Common labels for all Kubernetes objects |
| deployment | object | `{"affinity":{},"annotations":null,"containerPorts":null,"containerSecurityContext":null,"enabled":false,"envConfigMaps":null,"envMap":null,"envSecrets":null,"envVariables":null,"hostAliases":null,"initContainers":null,"labels":null,"lifecycle":null,"livenessProbe":null,"matchLabels":null,"nodeSelector":null,"readinessProbe":null,"replicas":1,"resources":{},"securityContext":null,"serviceAccount":{"enabled":false},"sidecar":null,"startupProbe":{},"strategy":"RollingUpdate","tolerations":null,"topologySpreadConstraints":null,"volumeMounts":null,"volumes":null}` | Deployment configuration |
| deployment.affinity | object | `{}` | Affinity rules for scheduling the pods |
| deployment.annotations | string | `nil` | Annotations for the Deployment |
| deployment.containerPorts | string | `nil` | Additional container ports |
| deployment.containerSecurityContext | string | `nil` | Security context for the container |
| deployment.enabled | bool | `false` | Whether to create a Deployment |
| deployment.envConfigMaps | string | `nil` | List of ConfigMap environment variables variable   - name of env variable inside container configMapName - name of kubernetes ConfigMap object configMapKey  - name of the key in ConfigMap object which holds the value |
| deployment.envMap | string | `nil` | Map of environment variables |
| deployment.envSecrets | string | `nil` | List of secret environment variables variable   - name of env variable inside container secretName - name of kubernetes secret object secretKey  - name of the key in secret object which holds the value |
| deployment.envVariables | string | `nil` | List of environment variables |
| deployment.hostAliases | string | `nil` | Host aliases for the pods |
| deployment.initContainers | string | `nil` | Init containers configuration |
| deployment.labels | string | `nil` | Labels for the Deployment |
| deployment.lifecycle | string | `nil` | Lifecycle hooks |
| deployment.livenessProbe | string | `nil` | Liveness probe configuration |
| deployment.matchLabels | string | `nil` | Match labels for the StatefulSet |
| deployment.nodeSelector | string | `nil` | Node selector for scheduling the pods |
| deployment.readinessProbe | string | `nil` | Readiness probe configuration |
| deployment.replicas | int | `1` | Number of replicas (ignored if .keda.enabled is true) |
| deployment.resources | object | `{}` | Resource requests and limits |
| deployment.securityContext | string | `nil` | Security context for the Deployment |
| deployment.serviceAccount | object | `{"enabled":false}` | Service account configuration |
| deployment.serviceAccount.enabled | bool | `false` | Whether to use the service account for deployment |
| deployment.sidecar | string | `nil` | Sidecar containers configuration |
| deployment.startupProbe | object | `{}` | Startup probe configuration |
| deployment.strategy | string | `"RollingUpdate"` | Deployment strategy |
| deployment.tolerations | string | `nil` | Tolerations for scheduling the pods |
| deployment.topologySpreadConstraints | string | `nil` | Topology spread constraints for scheduling the pods |
| deployment.volumeMounts | string | `nil` | Volume mounts for the container |
| deployment.volumes | string | `nil` | Volumes for the pod |
| image | object | `{"args":null,"command":null,"port":8080,"registry":"docker.io","repository":"nginx","tag":"1.0.0"}` | Docker image configuration |
| image.args | string | `nil` | Arguments to pass to the command |
| image.command | string | `nil` | Command to run in the Docker container |
| image.port | int | `8080` | Port the application will listen on (>1024) |
| image.registry | string | `"docker.io"` | Docker registry |
| image.repository | string | `"nginx"` | Docker image repository |
| image.tag | string | `"1.0.0"` | Docker image tag |
| namespaceOverride | string | `nil` | Override the default namespace |
| podDisruptionBudget | object | `{"enabled":false,"minAvailable":1}` | Pod Disruption Budget configuration |
| podDisruptionBudget.enabled | bool | `false` | Whether to create a Pod Disruption Budget |
| podDisruptionBudget.minAvailable | int | `1` | Minimum number of pods that must be available |
| serviceAccount | object | `{"annotations":null,"create":false,"labels":null}` | Service Account configuration |
| serviceAccount.annotations | string | `nil` | Annotations for the Service Account |
| serviceAccount.create | bool | `false` | Whether to create a Service Account |
| serviceAccount.labels | string | `nil` | Labels for the Service Account |