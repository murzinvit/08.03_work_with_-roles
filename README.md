08.03_work_with_-roles </br>
---------------------------</br>
Мои роли работают только из дистрибов kibana,elastic расположенных в локальных папках ролей - files. Переменные использовал всего 2, разнёс в default и vars в папках ролей.</br>
Роли ставяться из git - ansible-galaxy install -r requirements.yml -p roles/</br>
Команда выполняется успешено - ansible-playbook site.yml -i inventory/prod.yml</br>
Ссылка на elastic-role:</br>
    https://github.com/murzinvit/elastic-role.git</br>
Ссылка на kibana-role:</br>
    https://github.com/murzinvit/kibana-role.git</br>

