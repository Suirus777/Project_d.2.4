<h2>Задание D2.4.1 </h2>
1. Поднимите у себя локальный K8S-кластер с помощью Minikube. <br>
Ответ: Инструкция по установке Minikube Debian/Ubuntu в моем случаи Debian 10:<br>
a. Установка Docker <br> <br>
<code>#apt install -y docker docker.io </code> <br> <br>
b. Установка Docker-compose <br><br>
<code>#curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose </code> <br><br>
c. Установка Minikube <br><br>
<code>#curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 
#install minikube-linux-amd64 /usr/local/bin/minikube </code> <br><br>
d. Запускаем кластер Minikube <br> <br>
<code> #minikube start </code> <br> <br>
2. В кластере должно быть всего пять нод, одна из них должна быть Сontrol Plane-нода. <br>
Ответ: Для добавления нод в кластер Minikube используем команду:<br><br>
<code># minikube node add --worker "Name_Worker_node" </code> <br><br>
3. После того как ноды поднимутся, получите список всех нод в вашем локальном кластере. <br> <br>
<code> root@node:/home/odmin# minikube status
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured

minikube-m02
type: Worker
host: Running
kubelet: Running

minikube-m03
type: Worker
host: Running
kubelet: Running

minikube-m04
type: Worker
host: Running
kubelet: Running

minikube-m05
type: Worker
host: Running
kubelet: Running

minikube-m06
type: Worker
host: Running
kubelet: Running </code> <br> <br>

5. Все команды и вывод результатов выполнения этих команд отправьте ментору на проверку.

