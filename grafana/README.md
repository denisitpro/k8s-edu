# Description
* Install grafana use official docs - https://grafana.com/docs/grafana/latest/setup-grafana/installation/kubernetes/
* the file is divided into several and numbered for ease of debugging


# Changes
* create grafana local storage PV
* Worked node **w-01** create path /opt/grafana # todo set step to ansible prefly and unification path 
* change grafana service - load balancer to ClusterIP
* nginx ingress support grafana publish
