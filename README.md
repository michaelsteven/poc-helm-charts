# poc-helm-charts

Helm charts for proof of concepts that use the incubator/common helm helper chart.

## How to Install a Chart

Here is how to install a chart using the common pattern:

```
helm upgrade --install -f common/values.yaml -f <<microservice-name>>/values.yaml -f buildset-<<version>>.txt --version "1.0.0" --set "appVersion=1.0.0" --namespace "default" <<env_name>>-<<mcicroservice-name>> <<microservice-name>>
```

