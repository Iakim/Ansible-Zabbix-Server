# Ansible: Create a Zabbix Server

### Please note the following details:
#### Version of zabbix-server-mysql

      - name: Criando Tabelas no Banco
        shell: zcat /usr/share/doc/zabbix-server-mysql-3.0.10/create.sql.gz | mysql -uzabbix -pz@bb1x zabbix
 
 #### Version of zabbix latest package
 
     - name: Realizando download do pacote mais recente
       shell: wget http://repo.zabbix.com/zabbix/3.4/rhel/7/x86_64/zabbix-release-3.4-2.el7.noarch.rpm

#### Local of timezone
       - lineinfile:
           path: /etc/httpd/conf.d/zabbix.conf
           regexp: '^        # php_value date.timezone Europe/Riga'
           line: '        php_value date.timezone America/Sao_Paulo'

### Details:

#### user = zabbix
#### database name = zabbix
#### password = z@bb1x
