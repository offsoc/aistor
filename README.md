# AIStor

Hyperscale Object Store for AI

MinIO AIStor is designed to allow enterprises to consolidate all of
their data on a single, private cloud namespace. Architected using
the same principles as the hyperscalers, AIStor delivers performance
at scale at a fraction of the cost compared to the public cloud.

AIStor runs in Kubernetes.

## Pre-requisites

* An active Kubernetes environment running a [maintained version](https://kubernetes.io/releases/)
* [`kubectl` CLI tool](https://kubernetes.io/docs/tasks/tools/#kubectl)

### Environment

You can run AIStor on Kubernetes providers such as

- Redhat Openshift
- Google Kubernetes Engine
- Amazon Elastic Kubernetes Service
- Azure Kubernetes Service
- Upstream Kubernetes

Other Kubernetes providers may also work.

## Getting Started

1. Install AIStor with the following `kubectl` command

   ```shell
   kubectl apply -k https://min.io/k8s/aistor
   ```
   
or install with helm
   ```shell
   helm repo add aistor https://aistor.min.io/
   helm install --namespace aistor --create-namespace aistor aistor/aistor --set global.license=<your-license-key>
   ```
