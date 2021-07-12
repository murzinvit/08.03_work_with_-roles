08.03_work_with_-roles </br>
Мои роли работают только из дистрибов kibana,elastic расположенных в локальных папках ролей - files. Переменные использовал всего 2, разнёс в default и vars в папках ролей.
Роли ставяться из git - ansible-galaxy install -r requirements.yml -p roles/
Команда выполняется успешено - ansible-playbook site.yml -i inventory/prod.yml
