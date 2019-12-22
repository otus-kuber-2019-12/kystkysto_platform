# Выполнено ДЗ № 1

 - [x] Основное ДЗ
 - [x] Задание со *

## В процессе сделано:
 - Установлен kubctl
 - Установлен Minikube
 - Установлен Kubernetes Dashboard
 - Проверен k9s
 - Проверенны основные комманды kubectl
 - Настроен Deployment core-dns
 - Собран docker образ и помещен в публичный репозиторий
 - Создан манифест для запуска web сервера и расшраен volume с init контейнером
 - Установлен kube-forwarder
 - Собран образ сервиса frontend приложения Hipster Shop
 - Произведенна попытка запуска frontend сервиса на k8s
 - Исправлен манифест для запуска сервиса frontend

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

## PR checklist:
 - [x] Выставлен label с номером домашнего задания
 