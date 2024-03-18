# Description
* grafana-cm - create upstream to specific service and name space. Конфиграция nginx которая будет перенаправлять запросы к вашему сервису в my-grafana namespace`
* grafana-proxy - deploy deployment and service. Service usage nginx-ingress 

```commandline
Создание прокси-сервиса: Вы можете создать промежуточный сервис в том же namespace, что и Ingress, который будет работать как прокси и перенаправлять запросы к сервису в другом namespace.
```