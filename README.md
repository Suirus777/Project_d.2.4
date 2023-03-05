<h2>Задание D2.4.1 </h2>
1. Поднимите у себя локальный K8S-кластер с помощью Minikube. <br>
Ответ: Инструкция по установке Minikube Debian/Ubuntu в моем случаи Debian 10:<br>
a. Установка Docker <br> <br>
<code><b>#apt install -y docker docker.io </b></code> <br> <br>
b. Установка Docker-compose <br><br>
<code><b>#curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose </b></code> <br><br>
c. Установка Minikube <br><br>
<code> <b>#curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 
#install minikube-linux-amd64 /usr/local/bin/minikube </b></code> <br><br>
d. Запускаем кластер Minikube <br> <br>
<code> <b>#minikube start </b></code> <br> <br>
2. В кластере должно быть всего пять нод, одна из них должна быть Сontrol Plane-нода. <br>
Ответ: Для добавления нод в кластер Minikube используем команду:<br><br>
<code><b># minikube node add --worker "Name_Worker_node" </b></code> <br><br>
3. После того как ноды поднимутся, получите список всех нод в вашем локальном кластере. <br> 
Ответ: Список NODE<br>
<img src=https://github.com/Suirus777/Project_d.2.4/blob/main/Minikube_nodes.JPG><br>
Список pod <br>
<img src=https://github.com/Suirus777/Project_d.2.4/blob/main/Minikube_podes.JPG> <br>
4. Все команды и вывод результатов выполнения этих команд отправьте ментору на проверку. <br>
https://github.com/Suirus777/Project_d.2.4/edit/main/README.md <br>

<h2>Задание D2.4.2 </h2>
Описание: <br>
Сообщество Kubernetes объявило, что в конце 2021 года Docker в качестве среды выполнения контейнеров будет объявлен как устаревший и не будет использоваться в K8S-кластере. Но Kind, который поднимает K8S-кластер на Docker, говорит о том, что в отношении поддержки работы кластера K8S беспокоиться не стоит. <br><br>
Задание: <br><br>
Почему Kind говорит, что это изменение его не затронет? <br><br>
Ответ: 
