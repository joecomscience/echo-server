# Installation

Makesure that you already install `halm` on your machine.

```bash
helm install prometheus stable/prometheus --namespace ${namespace} --set alertmanager.persistentVolume.storageClass="gp2",server.persistentVolume.storageClass="gp2"
```

***Note*** If you got an error just run `helm repo update`.
