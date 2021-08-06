# kuber-14.3

задача 1

создал карты конфигурации nginx-config и domain

kubectl create configmap nginx-config --from-file=nginx.conf

kubectl create configmap domain --from-literal=name=netology.ru

посмотрел список карт

kubectl get configmaps

посмотрел детально карты

kubectl get configmap nginx-config

kubectl describe configmap domain

получил информацию в ямл и джейсон

kubectl get configmap nginx-config -o yam

kubectl get configmap domain -o json

выгрузил в файлы ямл и джейсон

kubectl get configmaps -o json > configmaps.json

kubectl get configmap nginx-config -o yaml > nginx-config.yml

удалил карту

kubectl delete configmap nginx-config

загрузил из файла

kubectl apply -f nginx-config.yml

запустил под netology-14.3

проверил подтянулись ли конфиги из карт


вторую задачу не делал

скрин в файле 1431.jpg

