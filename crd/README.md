## Local Knative Install using Skaffold

This example uses Knative's CRD to deploy. The [Installing Knative Serving using YAML files](https://knative.dev/docs/install/yaml-install/serving/install-serving-with-yaml/) instructions were used as an inspiration for this.

### Setup

- `make init` starts minikube
- `make install` installs the Knative operator into the knative-serving namespace
- `make run` deploys a Knative instance into the default namespace
- `minikube tunnel` allows access to deployed services from local

### Next Steps

Use [Func CLI](https://knative.dev/docs/functions/install-func/) or [Knative CLI](https://knative.dev/docs/client/install-kn/) to deploy services

### Additional Commands

- `make stop` removes currently deployed Knative serving instance
- `make clean` removes the minikube container and deletes the local Kubernetes environment
