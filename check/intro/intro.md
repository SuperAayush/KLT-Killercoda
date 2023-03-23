<br>


# Getting Started

The Keptn Lifecycle Toolkit (KLT) “wraps” a standard Kubernetes deployment and provides both workload (single service) tests and SLO evaluations. Multiple workloads can also be logically grouped (and evaluated) as a single cohesive unit: a Keptn Application. In other words, an application is a collection of multiple workloads.

The Keptn Lifecycle Toolkit is a tool and vendor-neutral mechanism - it does not depend on particular GitOps tooling - ArgoCD, Flux, Gitlab or others - KLT works with them all.

The Keptn Lifecycle Toolkit emits signals at every stage (k8s events, OpenTelemetry metrics and traces) to ensure your deployments are observable.

Available steps (applicable to both workload and application entities):

Pre-Deployment Tasks: e.g. checking for dependant services, checking if the cluster is ready for the deployment, etc.
Pre-Deployment Evaluations: e.g. evaluate metrics before your application gets deployed (e.g. layout of the cluster)
Post-Deployment Tasks: e.g. trigger a test, trigger a deployment to another cluster, etc.
Post-Deployment Evaluations: e.g. evaluate the deployment, evaluate the test results, etc.

## What you will learn here

Use the Keptn Lifecycle Toolkit to control the deployment of your application
Connect the lifecycle-toolkit to Prometheus
Use pre-deployment tasks to check if a dependency is met before deploying a workload
Use post-deployment tasks on an application level to send a notification

## Requirements 

A kubernetes cluster of more than the 1.24 version and kubectl installed
In this demo we already have this configured.

To check the version just run:

`kubectl version`{{exec}}


