# K8S-Sample

## Project Overview
The K8S-Sample repository contains a series of Kubernetes configuration files used to deploy and manage applications within a Kubernetes environment. Each file serves a specific purpose in the setup and management of Kubernetes resources, demonstrating best practices for organizing and managing Kubernetes deployments.

## Features
- **Namespace Management:** Create and manage Kubernetes namespaces.
- **Deployments:** Define and manage application deployments, including different deployment strategies.
- **Services:** Configure and manage various types of Kubernetes services.
- **Persistent Storage:** Manage persistent volumes and claims.
- **Configuration Management:** Use ConfigMaps and Secrets to manage configuration data.
- **Role-Based Access Control:** Define roles and role bindings for access control.
- **Health Checks:** Configure liveness and readiness probes to ensure application health.

## Requirements
- Kubernetes cluster
- kubectl installed and configured to interact with your cluster

## Installation

1. **Clone the repository:**
    ```sh
    git clone git@github.com:mohammadrezachegini/K8S-Sample.git
    cd K8S-Sample
    ```

2. **Apply the configurations:**
    ```sh
    kubectl apply -f <configuration-file>
    ```
    Replace `<configuration-file>` with the path to the desired configuration file.

## Usage

Each directory contains specific configuration files for different purposes. Below is an overview of each configuration file and its purpose.

### Namespace Configuration

- **ns.yaml:** Defines a Kubernetes namespace to logically separate resources.

### Deployments

- **deployment.yaml:** Main application deployment configuration.
- **deployment-blue.yaml:** Configuration for the blue version of the application.
- **deployment-green.yaml:** Configuration for the green version of the application.
- **deployment-red.yaml:** Configuration for the red version of the application.
- **deployment-yellow.yaml:** Configuration for the yellow version of the application.
- **deployment-ingress.yaml:** Configuration for the ingress associated with the deployment.

### ReplicaSets

- **replicaset.yaml:** Ensures a specified number of pod replicas are running at any given time.

### Services

- **postgres-svc.yaml:** Service configuration for PostgreSQL.
- **svc-clusterip.yaml:** ClusterIP service configuration for internal networking.
- **svc-nodeport.yaml:** NodePort service to allow external access to services.
- **svc-ingress.yaml:** Ingress service configuration for routing.

### Persistent Volumes and Claims

- **pv1.yaml, pv1-recycle.yaml:** Configuration for a persistent volume and its recycle policy.
- **pv2.yaml, pv2-recycle.yaml:** Another set of persistent volume configurations.
- **pv3.yaml, pv3-recycle.yaml:** Third set of persistent volume configurations.
- **pvc.yaml:** Persistent volume claim that requests storage.

### Configurations and Secrets

- **configMap.yaml, configMap2.yaml:** Maps of configuration settings that can be consumed by pods.
- **secretMap.yaml:** Example of how to store sensitive information.

### Roles and Role Bindings

- **anisa-role.yaml, anisa-role2.yaml:** Role configurations for specific permissions within the namespace.
- **anisa-cluster-role.yaml:** Cluster-wide role configuration.
- **role-binding.yaml:** Binds roles to specific users or groups.
- **cluster-role-binding.yaml:** Cluster-wide binding of roles.

### Health Checks

- **readiness.yaml:** Configuration for readiness probes.
- **liveness.yaml, liveness2.yaml:** Configurations for liveness probes.

### Miscellaneous

- **pod.yaml, pod-config-sh.yaml, pod-def.yaml:** Example pod configurations.
- **rslimit.yaml:** Limit resources like CPU and memory for containers.
- **role-binding.yaml:** Role binding details for Kubernetes roles.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Kubernetes Community
- Contributors and Supporters

## Troubleshooting
- **Connection Issues:** Ensure your `kubectl` context is set to the correct cluster.
- **Deployment Issues:** Check the status of pods and events in the namespace to identify issues.

## Contact
For any issues or questions, please open an issue in the repository or contact the repository owner.

## Screenshots

### Deployment Overview
![Deployment Overview](path/to/screenshot1.png)

### Service Configuration
![Service Configuration](path/to/screenshot2.png)

## Additional Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Kubectl Documentation](https://kubernetes.io/docs/reference/kubectl/)
- [Kubernetes Best Practices](https://kubernetes.io/docs/concepts/cluster-administration/networking/)
