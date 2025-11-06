### Переменные:

Для запуска плейбука необходимо указать параметры подключения к серверу, в файле конфигурации /host_vars/web_server_1.yml

```
ansible_host: ANSIBLE_HOST
ansible_user: ANSIBLE_USER
ansible_ssh_private_key_file: KEY_FILE_PATH
```
, где: 
ANSIBLE_HOST - адрес подключения к серверу
ANSIBLE_USER - пользователь с sudo правами
KEY_FILE_PATH - путь до ssh ключа. 

После указания переменных можно запустить плейбук командой: 
```
ansible-playbook prepare_server.yml
```