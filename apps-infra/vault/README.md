# Description
Deploy example vault cluster

# helm 3
* Security Warning: By default, the chart runs in standalone mode - https://developer.hashicorp.com/vault/docs/platform/k8s/helm/run

# Install use helmfile
`helmfile apply -f apps-infra/vault/helmfile-vault.yml`

# Install manifest
```
helm repo add hashicorp https://helm.releases.hashicorp.com
helm install vault hashicorp/vault
```

# Docs
* https://developer.hashicorp.com/vault/tutorials/kubernetes/kubernetes-raft-deployment-guide
* https://developer.hashicorp.com/vault/docs/platform/k8s/helm/run


# Step
* install helm chart
* create example local storage - 12Gi, chart need 10Gi
