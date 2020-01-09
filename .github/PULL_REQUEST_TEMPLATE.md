# Выполнено ДЗ № 3

 - [x] Основное ДЗ

## В процессе сделано:
 - Создан Service Account bob, который связан с кластерной ролью admin
 - Создан Service Account dave без доступа к кластеру
 - Создан Namespace prometheus
 - Создан Service Account carol в Namespace prometheus
 - Создана кластерная роль get-list-watch-pod и связанна со всеми Service Account в Namesspace prometheus
 - Создан Namespace dev
 - Создан Service Account jane
 - Service Account jane связан с ролью admin
 - Создан Service Account ken
 - Cвязанн Service Account ken и роль view

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

## PR checklist:
 - [x] Выставлен label с номером домашнего задания

 