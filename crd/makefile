.PHONY: init install run stop clean

init:
	minikube start --cpus 4 --memory 8192

install:
	skaffold run -p knative-install

run:
	skaffold run -p knative-deploy

stop:
	skaffold delete -p knative-deploy

clean:
	minikube delete
