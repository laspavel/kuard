# Kuard - тестовые поды для нагрузки кластера K8S

### Запуск:

```kubectl create namespace test1```
```kubectl config set-context --current --namespace=test1```
```kubectl apply -f deployment.yaml```
```kubectl apply -f service.yaml```
```kubectl apply -f ingress.yaml```

### На выходе:
```kubectl get pods```

### Удаление:
```kubectl delete ingress kuard```
```kubectl delete service kuard```
```kubectl delete deployment kuard```
```kubectl config set-context --current --namespace=default```
```kubectl delete namespace test1```



