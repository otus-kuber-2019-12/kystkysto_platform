# Выполнено ДЗ № 8

 - [x] Основное ДЗ
 - [ ] ДЗ со звездочкой

## В процессе сделано:
 - Собран docker образ с nginx
 - Prometheus operator установлен через helm 3
 - Написан Deployment для образа deocker c nginx и nginx exporter
 - Написан Service для nginx
 - Написан Service Monitor для nginx

## Как запустить проект:
 - Установка prometheus-operator
 ```bash
 kubectl create ns monitoring | helm install monitoring stable/prometheus-operator -n monitoring
 ```
 - Необходимо поочередно применить все манифесты:
 ```bash
 kubectl apply -f <имя файла содержащего манифест>
 ```
 
## PR checklist:
 - [x] Выставлен label с номером домашнего задания