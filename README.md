# rabbitmq

## Deploy Operator

```
kubectl apply -f "https://github.com/rabbitmq/cluster-operator/releases/latest/download/cluster-operator.yml"
```

## Create a RabbitMQ Instance
```yaml
    apiVersion: rabbitmq.com/v1beta1
    kind: RabbitmqCluster
    metadata:
        name: definition
```

# Set labels on nodes
```
kubectl label nodes worker-4 rabbitmq.ibits.co/node=rabbitmq
```