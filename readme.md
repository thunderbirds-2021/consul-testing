Raised an issue about ingress gateway in 
serverfault:https://serverfault.com/questions/1069357/how-to-configure-consul-to-access-webpage-from-ingress-gateway
hashicorp community: https://discuss.hashicorp.com/t/how-to-configure-consul-to-access-webpage-from-ingress-gateway/26636
github: https://github.com/hashicorp/consul/issues/10592

GEtting started guide link doesn't have ingress gateway added to the config.yaml for helm.
But this is availabe in this link https://www.consul.io/docs/k8s/connect/ingress-gateways
The same sample is added to the configuration of static-app folder.
Also, to allow traffic from any host instead of adding header in the above link, * is added to hosts as in this link: https://discuss.hashicorp.com/t/how-to-configure-consul-to-access-webpage-from-ingress-gateway/26636
