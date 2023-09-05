We will be using public Helm Chart:
-----
we will be using k8s 'metrics-server' helm chart:
https://artifacthub.io/packages/helm/metrics-server/metrics-server\

it is usually used for horizontal pod autoscalling

topo get CPU/RAM:
kubectl top pod
kubectl top node

-----
commands:
helm repo add metrics-server https://kubernetes-sigs.github.io/metrics-server/

helm show values metrics-server/metrics-server --version 3.8.4 > values.yaml


