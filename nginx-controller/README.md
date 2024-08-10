# example if LB create before
helm install nginx-ingress ingress-nginx/ingress-nginx \
  --namespace nginx-ingress \
  --set controller.replicaCount=2 \
  --set controller.service.externalIPs={1.2.3.4} \
  -f overwrite-affinity.yaml

# example LB not created
helm install nginx-ingress ingress-nginx/ingress-nginx \
  --namespace nginx-ingress \
  --set controller.replicaCount=2 