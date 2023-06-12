Задание 1:
1) создать docker compose файл, состоящий из 2 различных контейнеров: 1 - веб, 2 - БД
2) запустить docker compose файл
3) по итогу на БД контейнере должно быть 2 реплики, на админере должна быть 1 реплика. Всего должно получиться 3 контейнера
4) выводы зафиксировать

Задание 2*:
1) создать кластер и мастер и слейв ноды
2) задеплоить на ноду несколько экземляров какого0нибудь контейнера, например nginx

```
rust@GB:~$ sudo docker ps -a

[sudo] пароль для rust: 

CONTAINER ID   IMAGE             COMMAND                  CREATED              STATUS              PORTS                                       NAMES

21266bd2afaf   mariadb:10.10.2   "docker-entrypoint.s…"   About a minute ago   Up About a minute   3306/tcp                                    mariadb-db-1

fbb804f78d46   adminer:4.8.1     "entrypoint.sh php -…"   About a minute ago   Up About a minute   0.0.0.0:6080->8080/tcp, :::6080->8080/tcp   mariadb-adminer-1

bc47531f6170   mariadb:10.10.2   "docker-entrypoint.s…"   About a minute ago   Up About a minute   3306/tcp                                    mariadb-db-2

rust@GB:~$ 


```
![adminer](https://github.com/Ledsager/container_homework5/blob/main/adminer.PNG)

![node1](https://github.com/Ledsager/container_homework5/blob/main/node1.PNG)
![node2](https://github.com/Ledsager/container_homework5/blob/main/node2.PNG)
![node3](https://github.com/Ledsager/container_homework5/blob/main/node3.PNG)

Якупов Р.А. Урок 5. Docker Compose и Docker Swarm
