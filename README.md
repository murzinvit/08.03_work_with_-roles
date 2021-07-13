#### 08.03_work_with_-roles </br>
====================================</br>
Мои роли работают только из дистрибов kibana, elastic расположенных в локальных папках ролей - files. Переменные использовал всего 2,version и disthome,
разнёс в default и vars в папках ролей.</br>
Роли ставяться из git - `ansible-galaxy install -r requirements.yml -p roles`/</br>
На контейнерах centos и ubuntu выполняется успешено - `ansible-playbook site.yml -i inventory/prod.yml`</br>
В контейнеры перед запуском ansible по `docker exec -it ubuntu /bin/bash` - надо поставить sudo и python, закомитить.</br>
Ссылка на elastic-role:</br>
    [elastic-role](https://github.com/murzinvit/elastic-role.git) </br>
Ссылка на kibana-role:</br>
    [kibana-role](https://github.com/murzinvit/kibana-role.git) </br>

