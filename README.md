# GitOps

This repository houses the GitOps configuration for the Kubernetes cluster.

## Application Synchronization

ArgoCD is configured to use an ApplicationSet pattern. It first reads from the `root-appset.yaml` file, and then dynamically creates a distinct application for every folder nested under the `apps` directory. This ensures new workloads are automatically picked up and deployed to the cluster.
