# Installation

```bash
helm install -f grafana-values.yaml stable/grafana --generate-name
```

## Login

user: `admin`

Get password using below command

```bash
kubectl get secret --namespace prometheus ${grafana-secret} -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
```