Repo:
https://github.com/hashicorp/learn-consul-kubernetes.git

From folder:
learn-consul-kubernetes/service-mesh/deploy/hashicups/

config.yaml:
this need to be added to helm command, not to kubernetes directly.
ingress-gateway added as a feature to the one in original repo.

helm install -f config.yaml consul hashicorp/consul --version "0.31.1" -n consul
#if any changes later:
helm upgrade -f config.yaml consul hashicorp/consul --version "0.31.1" -n consul

Application install:
kubectl apply -f hashicups/


Create a zero trust network and individual services intentions using:
kubectl apply -f zero-trust-network/


These yaml files are created from the details mentioned in urls.
kubectl apply -f gateway_related/

Reference:
Getting started: https://learn.hashicorp.com/tutorials/consul/service-mesh-deploy?in=consul/gs-consul-service-mesh
Info related to gateway:
https://learn.hashicorp.com/tutorials/consul/service-mesh-traffic-management

Allow traffic from all hosts:
https://serverfault.com/questions/1069357/how-to-configure-consul-to-access-webpage-from-ingress-gateway
