Warning: WIP : documentation will come soon




## Purpose

Helm packaging of the microservices part of the web-terminal application

## Prerequisites

Make sure [cert-manager](https://cert-manager.io) is installed in the cluster before deploying the application.

## Deployment with Helmfile

First, clone the helm repository.

```bash
git clone https://github.com/w3term/helm.git
cd helm
```

Next, modify `values.yaml` according to your needs (more on that soon)

Next, verify the templates are correctly rendered.

```bash
helmfile templates
```

Then, deploy the application.

```bash
helmfile apply
```

## Removing the application

```bash
helmfile destroy
```