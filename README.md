#### 08.03_work_with_-roles </br>
====================================</br>
Загрузить контейнеры - `docker pull ubuntu:latest`, `docker pull centos:latest`. </br>
Запуск контейнеров для изменения - `docker run -d --name ubuntu ubuntu:latest sleep 10000000`, `docker run -d --name centos centos:latest sleep 10000000` </br> 
В контейнеры перед работой с ansible поставить sudo и python, зайдя в консоль - `docker exec -it ubuntu /bin/bash`, `docker exec -it centos /bin/bash`</br>
Закоментировать изменения в контейнерах - `docker commit -p ubuntu ubuntu:ver1`,  `docker commit -p centos centos:ver1`</br>
Роли работают только из дистрибутивов kibana, elastic расположенных в локальных папках ролей - files. </br>
Переменные использовал 2, - dist_version и dist_home, разнёс их в папки - default и vars, в папках ролей.</br>
Роли ставяться из git в папку roles, команда установки - `ansible-galaxy install -r requirements.yml -p roles/`</br>
Выполнение playbook - `ansible-playbook site.yml -i inventory/prod.yml`</br>

Ссылка на elastic-role:</br>
    [elastic-role](https://github.com/murzinvit/elastic-role.git) </br>
Ссылка на kibana-role:</br>
    [kibana-role](https://github.com/murzinvit/kibana-role.git) </br>

