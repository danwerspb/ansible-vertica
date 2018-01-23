Роль ансибл для утсановки Vertica DB

run:
ansible-playbook -i docker_hosts vertic.yaml

info:
ansible-vertica/roles/ansible-vertica/defaults/main.yml - параметры по умолчанию
Параметр run_mode отвечает за режим запуска - Deploy, Stop, Install, Start, Logging, or Recover

ansible-vertica/roles/ansible-vertica/README.md - readme оригинальной роли

В docker_hosts прописываем хосты с которыми будем работать. Необходимо что бы была авторизация по ключам с основной машины.

Возникают проблемы с размещением больших файлов в github. Deb пакет нужно скачать по ссылке https://yadi.sk/d/GH8PBjhO3RUoUu и положить в ansible-vertica/roles/ansible-vertica/files/vertica_9.0.1-0_amd64.deb. Либо регистрируемся и качаем официально. 

Протестировано на Ubuntu 16.04 и 14.04


Интерактивный запуск контейнера - docker exec -it <mycontainer> bash


