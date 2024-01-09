# Prometheus-for-kubernetes

## Installation

> ### Prerequisites

> - Kubernetes cluster access 

> - Kubectl utility

> - Helm 2.12+


### Step 1: Create a namespace for Prometheus resources and update the namespace in new-values.yml file.
> kubectl create ns monitoring

### Step 2: Add Helm Repo
> helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

### Step 3: Install Helm Chart with custom values mentioned in new-values.yml file.
> helm install prometheus prometheus-community/kube-prometheus-stack –f new-values.yml
