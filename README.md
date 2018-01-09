[![PyPI version](https://img.shields.io/pypi/v/ansible.svg)](https://pypi.python.org/pypi/ansible/2.4.2.0)
# Ansible playbook for install a Zabbix Server

### Please note the following detail:
- Local of timezone

       - lineinfile:
           path: /etc/httpd/conf.d/zabbix.conf
           regexp: '^        # php_value date.timezone Europe/Riga'
           line: '        php_value date.timezone America/Sao_Paulo'

- Details:

         user = zabbix
         database name = zabbix
         password = z@bb1x
         
- Visit https://www.zabbix.com/ for more details
