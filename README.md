
# k3s


curl -sfL https://get.k3s.io | sh - 


## Worker
curl -sfL https://get.k3s.io | K3S_URL=https://192.168.0.53:6443 K3S_TOKEN="K103548dbfb18a31faa2322a500d0716284c11b23247f1ed874f309d96223523735::server:4c0303807a550456e2cea0006daa5ba5" sh -


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

