## Local Knative Playground

This is my playground for learning Knative. It may or may not be helpful to you and should not be used in production.
The crd directory was my first attempt to spin up Knative using their CustomResourceDefinitions.
The operator directory is the prefered method to install Knative.

### Requirements
* [Minikube](https://minikube.sigs.k8s.io/docs/start/)
* [kubectl](https://kubectl.docs.kubernetes.io/installation/kubectl/)
* [Skaffold](https://skaffold.dev/docs/install/#standalone-binary)
* [Make](https://www.gnu.org/software/make/)

### Recommended
* [Knative CLI](https://knative.dev/docs/client/install-kn/) for managing Knative from the command line
* [Func CLI](https://knative.dev/docs/functions/install-func/) to create and deploy serverless functions
