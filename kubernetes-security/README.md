## Как запустить проект:
 - Необходимо поочередно применить все манифесты:
 ```bash
 kubectl apply -f <имя файла содержащего>
 ```

## Как проверить работоспособность:
 - Необходимо проверить все созданные привязки ролей:
 ```bash
kubectl get clusterrolebinding <имя биндинга> -o yaml
 ```