Clickhouse role
=========

Роль для установки clickhouse.

Requirements
------------

- ansible==9.3.0
- ansible-base==2.10.8
- ansible-core==2.16.4

Variables
--------------

Все перезаписываемые переменные в defaults/main.yml
| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
|clickhouse_version: | "22.3.3.44" | указывает версию кликхаус, необходимую для установки |
|download_path: | /home/vagrant | путь для выгрузки установочных пакетов|
|listen_ip: | 0.0.0.0 | ip адрес на котором будет прослушиваться интерфейс|

Example Playbook
----------------

Добавить в playbook:

    - hosts: servers
      roles:
         - { role: clickhouse-role }

License
-------

BSD

Author Information
------------------


