# cka-k8s
Kubernetes (also known as k8s or “kube”) is an open source container orchestration platform.
Released on 2015.
Scalable way to run containers on public cloud, on-prem data center or on your laptop.

Certifications:

CKAD(Certified Kubernetes Application Developer, Level 1)

CKA(Certified Kubernetes Administrator, Level 2

ETCD is a distributed reliable key-value store that is Simple, Secure & Fast

Namespaces:
1. Default
2. kube-system
3. kube-public

Usgae: service-name.namespace.service.domain
Ex. db-service.dev.svc.cluster.local
#kubectl get pods --namespace=namespace-name
#kubectl config set-context $(kubectl config current-context) --namespace=dev # To set dev as default namespace

TO LIMIT RESOURCES IN NAMESPACE - create ResourceQuota

SERVICES:
Enables communication within and outside of the applications.
External Communication: NodePort Service - Makes internal pod accessible on a port.
Cluster IP: Serive creates virtual IP between various sevices. 
Load Balancer: Provisions load balancer for load balancer in supported cloud provider.

IMPERATIVE: step by step instruction to reach destination.
DECLARATIVE: Direct final instruction to reach destination.

#kubectl get nodes
#kubectl get svc
#kubectl get pods
