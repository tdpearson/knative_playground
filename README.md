## Local Knative using minikube

This is my playground for learning Knative in a localy ran Kubernetes environment. It may or may not be helpful to you.
The crd directory was my first attempt to spin up Knative using their CustomResourceDefinitions. It also uses the kourier ingress server. See the [README](crd/README.md) for more details about deploying this version.

The operator directory installs Knative using the [Kubernetes operator pattern](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/). See the [README](operator/README.md) for more details about deploying this version.

Both subdirectories will install a functioning Knative environment using minikube for local development / experimentation.
Pick one at a time to deploy.

There is an easier way to install the Knative operator using a [CLI plugin](https://knative.dev/docs/install/operator/knative-with-operator-cli/) available on MacOS and Linux.

### Requirements

- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [kubectl](https://kubectl.docs.kubernetes.io/installation/kubectl/)
- [Skaffold](https://skaffold.dev/docs/install/#standalone-binary)
- [Make](https://www.gnu.org/software/make/)
- [httpie cli](https://httpie.io/cli)

### Recommended

- [Knative CLI](https://knative.dev/docs/client/install-kn/) for managing Knative from the command line
- [Func CLI](https://knative.dev/docs/functions/install-func/) to create and deploy serverless functions
