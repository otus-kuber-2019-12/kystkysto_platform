## Как запустить проект:
 - Первый сервис:
 ```bash
kubectl apply -f web-pod.yaml
kubectl port-forward --address 0.0.0.0 pod/web 8000:8000
 ```
 - Сервис frontend приложения Hipster Shop
 ```bash
 kubectl apply -f frontend-pod.yaml
 ```
  - Исправленый манифест сервиса frontend
 ```bash
 kubectl apply -f frontend-pod-healthy.yaml
 ```

## Как проверить работоспособность:
 - Перейти по ссылке http://localhost:8000 для проверки первого сервиса 
 - Проверить сервис frontend и его исправленную версию можно командой:
  ```bash
kubectl apply -f frontend-pod-healthy.yaml
 ```
