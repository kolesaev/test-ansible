# ActiveMQ для CentOS

### Описание

В данной ветке playbook вынесен в роль, в которой задачи разбиты на отдельные модули и подключены через include_tasks.

### Запуск

Для запуска на удалённых хостах требующих логин и пароль используется команда
```
ansible-playbook -v -i <хост>, playbook.yaml --extra-vars="ansible_user=<логин> ansible_password=<пароль>"
```

Для запуска по приватному ключу используется команда
```
ansible-playbook -v -i <хост>, playbook.yaml --private-key="<путь к приватному ключу>"
```