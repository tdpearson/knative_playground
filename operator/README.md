## Local Knative Install using Skaffold

This example uses Knative's K8S Operator to deploy.
Using Kourier for ingress.

### Setup
* `make init` starts minikube
* `make install` installs the Knative operator into the knative-serving namespace
* `make run` deploys a Knative instance into the default namespace
* `minikube tunnel` allows access to deployed services from local

### Next Steps
Use Func CLI or Knative CLI to deploy services

### Additional Commands
* `make stop` removes currently deployed Knative serving instance
* `make uninstall` removes the Knative operator
* `make clean` removes the minikube container and deletes the local Kubernetes environment


