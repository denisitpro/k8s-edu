# Docs
[1] https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-certs/#kubeconfig-additional-users

# Step by step full admmin
https://aungzanbaw.medium.com/a-step-by-step-guide-to-creating-users-in-kubernetes-6a5a2cfd8c71

# create user 1 week
```commandline
kubeadm kubeconfig user --config user.yaml --client-name user1 --validity-period 168h
```

# Step for create user admin-cluster  expire 1 week
* create admin account use kubeadm

`kubeadm kubeconfig user --config user.yaml --client-name admin1 --validity-period 168h`

Example code user.yaml (read official docs [1])
```commandline
apiVersion: kubeadm.k8s.io/v1beta3
kind: ClusterConfiguration
# Will be used as the target "cluster" in the kubeconfig
clusterName: "kubernetes"
# Will be used as the "server" (IP or DNS name) of this cluster in the kubeconfig
controlPlaneEndpoint: "k8s.beta-82.win:6443"
# The cluster CA key and certificate will be loaded from this local directory
certificatesDir: "/etc/kubernetes/pki"
```

* apply assign role for new user - cluster-admin-assign.yml