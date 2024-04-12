# Kubernetes Configuration Files

This repository contains a series of Kubernetes configuration files that are used to deploy and manage applications within a Kubernetes environment. Each file serves a specific purpose in the setup and management of Kubernetes resources.

### Namespace Configuration
- **ns.yaml**: Description of what this namespace configuration does.

### Deployments
- **deployment.yaml**: Main application deployment configuration.
- **deployment-blue.yaml**: Configuration for the blue version of the application.
- **deployment-green.yaml**: Configuration for the green version of the application.
- **deployment-red.yaml**: Configuration for the red version of the application.
- **deployment-yellow.yaml**: Configuration for the yellow version of the application.
- **deployment-ingress.yaml**: Configuration for the ingress associated with the deployment.

### ReplicaSets
- **replicaset.yaml**: Configuration for maintaining a stable set of replica Pods running at any given time.

### Services
- **postgres-svc.yaml**: Service configuration for PostgreSQL.
- **svc-clusterip.yaml**: ClusterIP service configuration for internal networking.
- **svc-nodeport.yaml**: NodePort service to allow external access to services.
- **svc-ingress.yaml**: Ingress service configuration for routing.

### Persistent Volumes and Claims
- **pv1.yaml**, **pv1-recycle.yaml**: Configuration for persistent volume and its recycle policy.
- **pv2.yaml**, **pv2-recycle.yaml**: Another set of persistent volume configurations.
- **pv3.yaml**, **pv3-recycle.yaml**: Third set of persistent volume configurations.
- **pvc.yaml**: Persistent volume claim that requests storage.

### Configurations and Secrets
- **configMap.yaml**, **configMap2.yaml**: Maps of configuration settings that can be consumed by pods.
- **secretMap.yaml**: Example of how to store sensitive information.

### Roles and Role Bindings
- **anisa-role.yaml**, **anisa-role2.yaml**: Role configurations for specific permissions within the namespace.
- **anisa-cluster-role.yaml**: Cluster-wide role configuration.
- **role-binding.yaml**: Binds roles to specific users or groups.
- **cluster-role-binding.yaml**: Cluster-wide binding of roles.

### Health Checks
- **readiness.yaml**: Configuration for readiness probes.
- **liveness.yaml**, **liveness2.yaml**: Configurations for liveness probes.

### Miscellaneous
- **pod.yaml**, **pod-config-sh.yaml**, **pod-def.yaml**: Example pod configurations.
- **rslimit.yaml**: Limit resources like CPU and memory for containers.
- **role-binding.yaml**: Role binding details for Kubernetes roles.
