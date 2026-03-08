# ML GitOps Kubernetes Manifests

This repository contains the **Kubernetes deployment manifests** for the ML GitOps Automation Platform.

The repository follows **GitOps principles**, where the Kubernetes cluster state is defined and managed through Git.

ArgoCD continuously monitors this repository and automatically synchronizes changes to the Kubernetes cluster.

---

## Contents

The repository contains Kubernetes configuration files including:

- Deployment configuration
- Service configuration
- Monitoring configuration
- Scaling configuration

These manifests define the desired state of the application running in the Kubernetes cluster.

---

## GitOps Workflow

1. CI pipeline builds a new Docker image
2. CI updates the image tag in the deployment manifest
3. Changes are pushed to this repository
4. ArgoCD detects the change
5. Kubernetes cluster is automatically synchronized

This enables **fully automated GitOps-based deployments**.

---

## Related Repositories

Application source code:

https://github.com/Krishna8934/ml-gitops-app

Full project documentation:

https://github.com/Krishna8934/ml-gitops-platform
