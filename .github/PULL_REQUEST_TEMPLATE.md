# Выполнено ДЗ № 4

 - [x] Основное ДЗ
 - [x] ДЗ со звездочкой

## В процессе сделано:
 - Создан minio StatefulSet
 - Создан minio HeadlessService
 - Добавлен Secret для хранения доступов к БД

## Как запустить проект:
 - Необходимо поочередно применить все манифесты:
 ```bash
 kubectl apply -f <имя файла содержащего>
 ```

## Как проверить работоспособность:
 - Необходимо проверить настройку следующими командами:
 ```bash
kubectl get statefulsets
kubectl get pods
kubectl get pvc
kubectl get pv
kubectl describe <resource> <resource_name>
 ```

## PR checklist:
 - [x] Выставлен label с номером домашнего задания

 