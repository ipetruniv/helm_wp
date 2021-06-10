helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
helm repo add stable https://charts.helm.sh/stable
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update


helm install wordpress bitnami/wordpress  -f ./values.yaml

When pods are ready, get external IP (kubectl get svc) and create DNS recod for site or update local hosts file
