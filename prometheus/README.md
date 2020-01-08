# Installation

Makesure that you already install `halm` on your machine.

```bash
helm repo add stable https://kubernetes-charts.storage.googleapis.com
helm install ${helm_name} stable/prometheus --namespace ${namespace} --set alertmanager.persistentVolume.storageClass="gp2",server.persistentVolume.storageClass="gp2"
```

***Note*** If you got an error just run `helm repo update`.
