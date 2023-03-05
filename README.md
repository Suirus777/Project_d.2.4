<h2>Задание D2.4.1 </h2>
1. Поднимите у себя локальный K8S-кластер с помощью Minikube. <br>
Ответ: Инструкция по установке Minikube Debian/Ubuntu в моем случаи Debian 10:
Установка Docker 

#apt install -y docker docker.io

Установка Docker-compose

#curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

Установка Minikube

#curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

#install minikube-linux-amd64 /usr/local/bin/minikube

Запускаем кластер Minikube
 
#minikube start
В кластере должно быть всего пять нод, одна из них должна быть Сontrol Plane-нода.
После того как ноды поднимутся, получите список всех нод в вашем локальном кластере.
Все команды и вывод результатов выполнения этих команд отправьте ментору на проверку.

