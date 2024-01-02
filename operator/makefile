.PHONY: all init install uninstall run stop clean

all: init install run

init: base/manifests/serving-default-domain.yaml base/manifests/operator.yaml
	minikube start --cpus 4 --memory 8192

install:
	skaffold run -p knative-install

uninstall:
	skaffold delete -p knative-install

run:
	skaffold run -p knative-deploy

stop:
	skaffold delete -p knative-deploy

clean:
	minikube delete
	rm -rf base/manifests

base/manifests/serving-default-domain.yaml:
	mkdir -p base/manifests
	http --download --output base/manifests/serving-default-domain.yaml get https://github.com/knative/serving/releases/download/knative-v1.12.3/serving-default-domain.yaml

base/manifests/operator.yaml:
	mkdir -p base/manifests
	http --download --output base/manifests/operator.yaml get https://github.com/knative/operator/releases/download/knative-v1.11.12/operator.yaml