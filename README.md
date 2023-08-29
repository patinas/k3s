
# k3s


curl -sfL https://get.k3s.io | sh - 


sudo cat /var/lib/rancher/k3s/server/node-token



## Worker
curl -sfL https://get.k3s.io | K3S_URL=https://[IP]:6443 K3S_TOKEN="[TOKEN]" sh -


# Helm

curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash



# Longhorn
## get charts
helm repo add longhorn https://charts.longhorn.io

## update
helm repo update

## install
helm upgrade -i longhorn longhorn/longhorn --namespace longhorn-system --create-namespace







### export KUBECONFIG="/etc/rancher/k3s/k3s.yaml"

