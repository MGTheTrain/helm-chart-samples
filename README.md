# helm-chart-and-kustomization-samples

## Table of Contents

+ [Summary](#summary)
+ [Features](#features)

## Summary

Helm Chart and Kustomization samples required in combination with the [gitops-poc Github repository](https://github.com/MGTheTrain/gitops-poc) to showcase GitOps. ArgoCD applications or Flux Kustomization will refer to these custom Helm Chart samples or Kustomizations samples. GitOps will be demonstrated in that the defined state of the Helm Charts or Kustomizations for the `main` branch synchronizes with the Kubernetes cluster via the **Sync Controller**.

**Remark:** It's generally not recommended to tightly bind backend service source code with Helm charts. Instead, it's common practice to have the Helm chart reference the built artifact (e.g., Docker image) of the backend service. This allows the backend service to evolve independently of the Helm chart, and simplifies the deployment process. This repository is solely for demonstrating GitOps.

## Features

- [x] Sample C# ASP .NET Core HelloWorld service 
- [x] CD wofklow for on demand deployments of an ACR (**Required for storing docker images**)
- [x] CI workflow for building and pushing the dockerized sample service to an ACR
- [x] Sample service and nginx helm chart required for GitOps
