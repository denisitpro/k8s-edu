# Docs
https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-certs/#kubeconfig-additional-users

# Step by step full admmin
https://aungzanbaw.medium.com/a-step-by-step-guide-to-creating-users-in-kubernetes-6a5a2cfd8c71

# create user 1 week
```commandline
kubeadm kubeconfig user --config user.yaml --client-name user1 --validity-period 168h
```

