## Install Helm

choco install kubernetes-helm

## Add contour

helm repo add bitnami https://charts.bitnami.com/bitnami
helm install my-release bitnami/contour --namespace projectcontour --create-namespace

## Add gateway CRD

kubectl apply -f https://github.com/kubernetes-sigs/gateway-api/releases/download/v1.0.0/standard-install.yaml