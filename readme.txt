плейбук на ансибл
проинсталлировать вертику на какой то хост
системные параметры изменять
задание считается выполненным если база установлена физически
admintool уже поднимает базу

run:
ansible-playbook -i docker_hosts vertic.yaml

info:
ansible-vertica-role/roles/ansible-vertica/defaults/main.yml - параметры по умолчанию
Параметр run_mode отвечает за режим запуска - Deploy, Stop, Install, Start, Logging, or Recover

ansible-vertica-role/roles/ansible-vertica/files/vertica_9.0.1-0_amd64.deb - дистрибутив Vertica

ansible-vertica-role/roles/ansible-vertica/README.md - readme оригинальной роли

В docker_hosts прописываем хосты. Необхдимо что бы была авторизация по ключам с основной машины.




