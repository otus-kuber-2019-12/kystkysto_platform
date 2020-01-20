## Как запустить проект:
 - Необходимо поочередно применить все манифесты:
 ```bash
 kubectl apply -f <имя файла содержащего манифест>
 ```

## Как проверить работоспособность:
 - Можно использовать kubespy и отслеживать изменения.
 - Пинговать ip кластера и запрашивать 80 порты для проверки доступноcти http