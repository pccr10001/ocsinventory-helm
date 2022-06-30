# Helm chart for OCS Inventory
### Installation
* copy `ocsi-secrets.yaml.sample` to `ocsi-secrets.yaml`
* modify secrets in `ocsi-secrets.yaml`
* modify configs in `values.yaml`
```
$ kubectl create namespace ocsinventory
$ kubectl apply -f ocsi-secrets.yaml
$ helm install -f .\Chart.yaml ocsinventory .
```