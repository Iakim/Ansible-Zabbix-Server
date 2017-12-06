# Ansible: Create a Zabbix Server

### Please note the following detail:
#### Local of timezone
       - lineinfile:
           path: /etc/httpd/conf.d/zabbix.conf
           regexp: '^        # php_value date.timezone Europe/Riga'
           line: '        php_value date.timezone America/Sao_Paulo'

### Details:
    user = zabbix
    database name = zabbix
    password = z@bb1x
